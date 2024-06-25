//Задача1.
#include <iostream>
#include <cmath>

int main() {
    double y = pow(2 * sqrt(5), 2) / 10;

    std::cout << "Значение выражения y = (5 * sqrt(2))^2 / 10 равно: " << y << std::endl;

    return 0;
}

//Задача2.
#include <iostream>
using namespace std;

// Функция для вычисления суммы первых n членов арифметической прогрессии
double arithmeticProgressionSum(double a1, double d, int n) {
    // Вычисляем сумму S_n
    double Sn = (n / 2.0) * (2 * a1 + (n - 1) * d);
    return Sn;
}

int main() {
    double a1, d;
    int n;

    // Ввод данных
    cout << "Введите первый член арифметической прогрессии a1: ";
    cin >> a1;
    cout << "Введите разность d: ";
    cin >> d;
    cout << "Введите количество членов n: ";
    cin >> n;

    // Вычисление суммы первых n членов арифметической прогрессии
    double Sn = arithmeticProgressionSum(a1, d, n);

    // Вывод результата
    cout << "Сумма первых " << n << " членов арифметической прогрессии: " << Sn << endl;

    return 0;
}

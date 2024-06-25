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
//Задача3.
#include <iostream>
#include <cmath> // Для использования sqrt()

using namespace std;

double averageSquareRoot(int a, int b, int c) {
    // Вычисляем среднее квадратичное
    double avg_sqrt = sqrt((pow(a, 2) + pow(b, 2) + pow(c, 2)) / 3.0);
    return avg_sqrt;
}

int main() {
    int num1 = 2, num2 = 11, num3 = 5;

    // Вычисляем среднее квадратичное чисел 2, 11 и 5
    double avg_sqrt = averageSquareRoot(num1, num2, num3);

    // Вывод результата
    cout << "Среднее квадратичное чисел " << num1 << ", " << num2 << " и " << num3 << " равно: " << avg_sqrt << endl;

    return 0;
} 

//Задача4.
#include <iostream>
using namespace std;

int main() {
    // Заданные данные
    double retailPrice = 180.0; // розничная цена
    double markupPercent = 20.0; // процент наценки

    // Вычисление оптовой цены
    double wholesalePrice = retailPrice / (1 + markupPercent / 100.0);

    // Определение максимального числа учебников, которые можно купить на 10000 рублей
    double totalMoney = 10000.0;
    int maxBooks = static_cast<int>(totalMoney / wholesalePrice);

    // Вывод результата
    cout << "Оптовая цена учебника: " << wholesalePrice << " рублей" << endl;
    cout << "Наибольшее число учебников, которое можно купить за 10000 рублей: " << maxBooks << endl;

    return 0;
}

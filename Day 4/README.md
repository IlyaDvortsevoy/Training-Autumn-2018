## Читать
- [C# 5.0 Unleashed. Bart De Smet. Sams Publishing. 2013](https://www.goodreads.com/book/show/16284093-c-5-0-unleashed)
    - *Chapter 10:* Methods
- [CLR via C#. Jeffrey Richter. Microsoft Press. 2010](https://www.goodreads.com/book/show/7121415-clr-via-c)
    - *Chapter 8:* Methods

## Материалы (презентация)
- [Methods in details](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M4.%20Methods%20in%20details)
- [LINQPad примеры](https://drive.google.com/drive/u/0/folders/1L4i-cL27xBQSlVcdzzx6PnCiUyzlwMfW)

## Задачи 
1. (deadline 18.10.2018, 24.00) Расширить функциональную возможность типа System.Double, реализовав возможность получения строкового представления вещественного числа в формате IEEE 754. Готовые классы-конверторы не использовать. Разработать модульные тесты. Примерные тест-кейсы
    - [TestCase(-255.255, ExpectedResult = "1100000001101111111010000010100011110101110000101000111101011100")]
    - [TestCase(255.255, ExpectedResult = "0100000001101111111010000010100011110101110000101000111101011100")]
    - [TestCase(4294967295.0, ExpectedResult = "0100000111101111111111111111111111111111111000000000000000000000")]
    - [TestCase(double.MinValue, ExpectedResult = "1111111111101111111111111111111111111111111111111111111111111111")]
    - [TestCase(double.MaxValue, ExpectedResult = "0111111111101111111111111111111111111111111111111111111111111111")]
    - [TestCase(double.Epsilon, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000001")]
    - [TestCase(double.NaN, ExpectedResult = "1111111111111000000000000000000000000000000000000000000000000000")]
    - [TestCase(double.NegativeInfinity, ExpectedResult = "1111111111110000000000000000000000000000000000000000000000000000")]
    - [TestCase(double.PositiveInfinity, ExpectedResult = "0111111111110000000000000000000000000000000000000000000000000000")]
    - [TestCase(-0.0, ExpectedResult = "1000000000000000000000000000000000000000000000000000000000000000")]
    - [TestCase(0.0, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000000")] и т.д.
2. (deadline 19.10.2018, 24.00) Реализовать метод TransformToWords который принимает массив вещественных чисел и трансформирует его в массив строк таким образом, чтобы каждое вещественное число преобразовывалось в его "словестный формат" (LINQ-запросы не использовать!). Например, FilterDigit (-23.809, 0.295, 15.17) -> {"minus two three point eight zero nine", "zero point two nine five", "one five point one seven"}. Разработать модульные тесты (NUnit или MS Unit Test) для тестирования метода.
3. (deadline 20.10.2018, 24.00) Разработать класс, позволяющий выполнять вычисления НОД по алгоритму Евклида для двух, трех и т.д. целых чисел (http://en.wikipedia.org/wiki/Euclidean_algorithm , https://habrahabr.ru/post/205106/, https://habrahabr.ru/post/205106/ ). Методы класса помимо вычисления НОД должны предоставлять дополнительную возможность определения значение времени, необходимое для выполнения расчета. Добавить к разработанному классу методы, реализующие алгоритм Стейна (бинарный алгоритм Евклида) для расчета НОД двух, трех и т.д. целых чисел (http://en.wikipedia.org/wiki/Binary_GCD_algorithm, https://habrahabr.ru/post/205106/ ), а также методы,  предоставляющие дополнительную возможность определения значение времени, необходимое для выполнения расчета. Рассмотреть различные возможности реализации методов, возвращающих время вычисления НОД. Разработать модульные тесты.

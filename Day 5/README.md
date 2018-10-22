## Читать
- [C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 3.* Creating Types in C#
- [C# 5.0 Unleashed. Bart De Smet. Sams Publishing. 2013.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 9.* Introducing Types

## Материалы (презентация)
- [Basic Coding in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M4.%20Methods%20in%20details)
- [Creating types in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M3.%20Creating%20types%20in%20C%23)
- [LINQPad примеры](https://drive.google.com/drive/folders/1GiBzgWWg9DmdOQq15H2YHuXMqN4uMaDv)

## Задачи
- (**переделка**) Реализовать метод расширения для получения строкового двоичного представления вещественного числа двойной точности в формате IEEE 754 (**при реализации готовые  классы-конверторы не использовать!**). Разработать модульные тесты. (NUnit фреймворк)
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
  - [TestCase(0.0, ExpectedResult = "0000000000000000000000000000000000000000000000000000000000000000")]   
и т.д.
      ![К решению](https://github.com/AnzhelikaKravchuk/Training-Summer-Express-2018/blob/master/Pictures/ToIEEE754.png) 
- (**deadline - 24.00 23.10.2018**) Разработать неизменяемый класс Polynomial (полином) для работы с многочленами степени  от одной переменной вещественного типа (в качестве внутренней структуры для хранения коэффициентов использовать sz-массив). Для разработанного класса переопределить виртуальные методы класса Object; перегрузить операции, допустимые для работы с многочленами (исключая деление многочлена на многочлен), включая "==" и "!=". Разработать unit-тесты (NUnit фреймворк).
- (**deadline - 24.00 22.10.2018**) Добавить в класс ([задание 1](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/tree/master/Day%204)) метод TransformToIEEEFormat который принимает массив вещественных чисел и трансформирует его в массив строк таким образом, чтобы каждое вещественное число преобразовывалось в его строковый формат IEEE 754.

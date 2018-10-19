## Читать
- [C# 6.0 in a Nutshell. Joseph Albahari, Ben Albahari. O'Reilly Media. 2015.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 3.* Creating Types in C#
- [C# 5.0 Unleashed. Bart De Smet. Sams Publishing. 2013.](https://drive.google.com/drive/u/0/folders/0B7WmjuqYed3Aeko0MzNYZWtVOUk)
   - *Chapter 9.* Introducing Types
- [Инкапсуляция. Наследование. Полиморфизм](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M6.%20Encapsulation.%20Inheritance.%20Polymorphism)

## Материалы (презентация)
- [Basic Coding in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M4.%20Methods%20in%20details)
- [Creating types in C#](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M3.%20Creating%20types%20in%20C%23)
- [LINQPad примеры](https://drive.google.com/drive/u/0/folders/18XpZW-YQWksZNoWTgaYnsp9IAhROdvD5)
- [Инкапсуляция. Наследование. Полиморфизм](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M6.%20Encapsulation.%20Inheritance.%20Polymorphism)

## Задачи

- (**deadline - 18.00 07.07.2018**) Реализовать метод расширения получения из строкового представления целого положительного четырехбайтового числа, записанного в p-ичной системе счисления (2<=p<=16), его десятичного значения (**при реализации готовые классы-конверторы не использовать!**). Разработать модульные тесты. (NUnit фреймворк). Примерные тесткейсы.
    - "0110111101100001100001010111111" для основания 2 -> 934331071
    - "01101111011001100001010111111" для основания 2 -> 233620159
    - "11101101111011001100001010" для основания 2 -> 62370570
    - "1AeF101" для основания 2 -> ArgumentException
    - "11111111111111111111111111111111" для основания 2 -> OverflowException
    - "1AeF101" для основания 16 -> 28242177
    - "1ACB67" для основания 16 -> 1756007
    - "SA123" для основания 2 -> ArgumentException
    - "764241" для основания 8 -> 256161   
    - "764241" для основания 20 -> ArgumentException  
    - "10" для основания 5 -> 5   
  и т.д.   

- (**deadline - 18.00 08.07.2018**) Разработать неизменяемый класс Polynomial (полином) для работы с многочленами степени  от одной переменной вещественного типа (в качестве внутренней структуры для хранения коэффициентов использовать sz-массив). Для разработанного класса переопределить виртуальные методы класса Object; перегрузить операции, допустимые для работы с многочленами (исключая деление многочлена на многочлен), включая "==" и "!=". Разработать unit-тесты (NUnit фреймворк).

## Читать
- [Object Oriented Design Principles](https://github.com/EPM-RD-NETLAB/.NET-Framework-modules/tree/master/M16.%20Object%20Oriented%20Design%20Principles)
- ***[Примеры использования Moq](https://habr.com/post/150859/)***
- ***[Moq.Quickstart](https://github.com/Moq/moq4/wiki/Quickstart)***
- [The Art of Unit Testing: with examples in C# Second Edition Edition. Roy Osherove.  Manning Publications Co. 2013.](https://www.manning.com/books/the-art-of-unit-testing-second-edition)
   - *Chapter 3.* [Using stubs to break dependencies](https://livebook.manning.com/#!/book/the-art-of-unit-testing-second-edition/chapter-3/1)
   - *Chapter 4.* [Interaction testing using mock objects](https://livebook.manning.com/#!/book/the-art-of-unit-testing-second-edition/chapter-4/1)

## Материалы (презентация)
- [Принципы проектирования. Материалы и примеры LINQPad](https://drive.google.com/drive/u/0/folders/1GfV5bnT8vZZZBxaccL4wl-ixXOH9Zc-i)
- [SOLID](https://drive.google.com/drive/u/0/folders/1Cu4GJDy2AOn0lbKXz2c7DgxOTXzT8NDh)
- [Project architecture](https://drive.google.com/drive/u/0/folders/1nuD42hcc84zDm2wea43gPjcdDrD3YwM5)
- [Примеры использования Moq (к статье выше)](https://drive.google.com/drive/u/0/folders/1nuD42hcc84zDm2wea43gPjcdDrD3YwM5)
- [Проект здесь](https://github.com/EPM-RD-NETLAB/Project-Arch)

## Задачи
0. Обязательно разобрать все, что касается mock-тестирования (см. ссылки выше). Протестировать (NUnit и Moq фреймворки) [проект](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/tree/master/Day%2019).
1. **(deadline - 02.12.2018, 18.00)** Создать обобщенные классы для представления квадратной, симметрической и диагональной матриц (симметрическая матрица – это квадратная матрица, которая совпадает с транспонированной к ней; диагональная матрица – это квадратная матрица, у которой элементы вне главной диагонали имеют значения по умолчанию типа элемента). Описать в созданных классах событие, которое происходит при изменении элемента матрицы с индексами (i, j).  Расширить функциональность существующей иерархии классов, добавив возможность операции сложения двух матриц любого типа. Разработать unit-тесты.

2. **(deadline - )** Разработать систему типов для описания работы с банковским счетом. Состояние счета определяется его номером, данными о владельце счета (имя, фамилия, e-mail), суммой на счете и некоторыми бонусными баллами, которые увеличиваются/уменьшаются каждый раз при пополнении счета/списании со счета на величины различные для пополнения и списания и рассчитываемые в зависимости от некоторых значений величин «стоимости» баланса и «стоимости» пополнения. Величины «стоимости» баланса и «стоимости» пополнения являются целочисленными значениями и зависят от типа счета, который может быть, например,  Base, Gold, Platinum. Для работы со счетом реализовать следующие возможности: 
   - выполнить пополнение на счет;
   - выполнить списание со счета; 
   - перевести сумму на другой счет;
   - создать новый счет; 
   - закрыть счет.    
    
    При проектировании типов учитывать следующие возможности расширения/изменения функциональности
      - добавление новых видов счетов;
      - изменение/добавление источников хранения информации о счетах;
      - изменение расчета бонусных баллов в производных классах;
      - изменении логики генерации номера счета.
    
    Для хранения информации о счетах использовать fake-имплементацию репозитория (хранилища) в виде класса-обертки для коллекции List<Account>.
 
    Работу классов продемонстрировать на примере консольного приложения. 
  
    Для организации классов и интерфейсов использовать “The Stairway pattern” (“заготовка” в архиве [AccountSystemDemo.7z](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/tree/master/Days%2020-23), пример [ProjectArchitectureDemo.7z](https://drive.google.com/drive/u/0/folders/1nuD42hcc84zDm2wea43gPjcdDrD3YwM5)). 
  
    Для разрешения зависимостей использовать Ninject- фреймворк.
    
    Реализовать возможность логирования сообщений различного уровня (NLog - фреймворк), предусмотрев возможность использования различных фреймворков для логирования. 

    Протестировать слой Bll (NUnit и Moq фреймворки).

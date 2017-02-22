# Задачи для начинающих программистов

Цель этих задач - развить навык мышления у студентов, которые уже умеют верстать, немного знакомы с синтаксисом js, но не могут еще писать программы. 

## 1. Задачи на ознакомление с синтаксисом

### 1.1 Массивы
Создать и вывести на экран два массива, один содержащий дни недели, а второй - месяцы. 

### 1.2 Объекты
Создать и вывести на экран объекты, в которых будет содержаться описание следуюущих объектов:
* вы сами (имя, год рождения, почта, телефон, семейное положение, профессия и т.п.)
* вашей квартиры или дома (сколько комнат, есть ли телефон, на каком этаже расположена и т.п)
* телефона (бренд, объем памяти, сколько симок поддерживает и т.п.)
* города (название, количество жителей, географические координаты, есть ли метро и выход к морю и т.п)

Подумайте о том, какие типы данных (строки, числа, булевые) могут быть использованя для каждого значения.
Подумайте, какие еще объекты из повседневной жизни вы могли бы описать.

## 2. Математические 

### 2.1 Цельсии в Фаренгейты
Написать функцию, которая будет конвертировать температуру из шкалы цельсия в шкалу фаренгейта. Функция принимает один аргумент - температуру в цельсиях, и возвращает значение в фаренгейтах. Расчет производится по следующей формуле: 

F = (C*9 / 5) + 32;
Пример вызова функции 

    convert(0); 
    =>  32

Добавить функцию, которая будет делать обратный расчет - из Фаренгейтов в Цельсии.

### 2.2 Перевод инчей в сантиметры
Написать функцию, которая будет конвертировать длину из инчей в сантиметры. Пользователь вводит длину в инчах, получает результат в сантиметрах.

Добавить функцию, которая будет переводить сантиметры в инчи

### 2.3 Площадь круга

Создать функцию, которая будет считать площадь круга, имея радиус. Формула для расчета: S = r*r*PI. PI можно считать равным 3,14. Функция принимает радиус как аргумент и возвращает площадь.

### 2.4 Лет, месяцев, дней
Функция принимает число дней, нужно определить, сколько это лет, месяцев и дней.
Условно год считаем за 365 дней, а месяц - за тридцать. 

Например,  450 дней это 1 год, 2 месяца, 25 дней.

    calculateTime(450);
    => "1 год, 2 месяца, 25 дней"

## 4. Условия

### 4.1 Разделение Нлогонии

После нескольких лет горячих споров о территории, жители страны Нлогонии решили разделить страну на 4 части. Все согласились, что будет определена Точка Раздела, от которой на карте будут проведены две линиии - одна с севера на юг, другая с востока на запад. Начиная с самой западной и самой северной, по часовой стрелке, страны будут называться Северозападна Нлогония, Северовосточная Нлогония, Юговосточная нлогония и Югозападная Нлогония.

ООН решило, что будет существовать страница в интернете, где жители смогут определить, в какой стране теперь находятся их дома. Вас наняли реализовать этот проект. 

![alt tag](https://uva.onlinejudge.org/contests/204-2cceaeb5/p11498.png)


Ввод:
В программе есть один объект, определяющий точку раздела:

    var border = {
      x : 12,
      y : 6
    }
    
И вы можете создавать разные объекты домов, у которых будут свои координаты местоположения:

    var house = { 
      x: -8,
      y: 35
    }
    
Попробуйте проделать то же самое с разными числами в объекте house

Вывод:
Вы должны вывести результат:

* border - если дом находится на границе
* NW - если дом находится в северо-западной части страны (NW = North West)
* NE - если дом находится в северо-восточной части страны (NE = North East)
* SW - если дом находится в юго-западной части страны (SW = South West)
* SE - если дом находится в юго--восточной части страны (SE = South East)


### 4.2 Max и Min
Написать две функции maxNumber и minNumber, обе принимают два числа, первая возвращает большее из двух, вторая возвращает меньшее из двух.

    minNumber(-3, 8);
    => -3
    maxNumber(-3, 8);
    => 8

### 4.3 Добрый Вечер!
Напишите функцию sayHello, которая будет выводить в консоль приветствие в зависимости от времени суток. Функция принимает в себя один аргумент - время в часах, от 0 до 23. 

    sayHello(8)
    => “Доброе утро!”
    sayHello(18) 
    => “Добрые вечер”
    
### 4.4 Error/Ошибка/Ката
Представим, что наш сайт может работать на трех языках, русском, английском и кыргызском. И во всех трех случаях мы должны выводить пользователю сообщение об ошибке на его языке. 

Напишите функцию printError, которая принимает в себя один аргумент - строку (“ru”, “en” или “kg”), и для каждого из языков печатает свое сообщение об ошибке.  

    printError(“en”) 
    “Error”
    printError(“kg”)
    “Ката”

### 4.5 Валидация пароля
По правилам безопасности, пароль пользователя должен быть не короче 6 символов. Напишите функцию, которая принимает один аргумент - строку, и проверяет ее длину. Если строка короче 6 символов, выводится сообщение об ошибке (“Пароль не может быть короче 6 символов”), если нет - то выводится сообщение(“Безопасный пароль”) 

## 5 Циклы:


### 5.1 Сообщение в рамочке

Написать функцию, которая принимает в себя одну строку, и выводит ее в прямоугольнике из звездочек

    *****************
    * Hello, world *
    *****************

### 5.2 Корзина
Создайте объект корзины, в котором будут храниться товары, укаждого есть цена и название

    var basket = {
      bread: 16,
      butter: 70
    }

Нужно написать функцию, которая посчитает общую сумму товаров в корзине.
  
    calculateTotal(basket);
    => 86

### 5.3 Max и Min в массиве
Написать две функции max и min, обе принимают один массив, первая возвращает самое большое число в массиве, вторая возвращает самое маленькое число в массиве.

### 5.4 FizzBuzz

Напишите программу, которая выводит через console.log все числа от 1 до 100, с двумя исключениями. Для чисел, нацело делящихся на 3, она должна выводить ‘Fizz’, а для чисел, делящихся на 5 (но не на 3) – ‘Buzz’. 

Когда сумеете – исправьте её так, чтобы она выводила «FizzBuzz» для всех чисел, которые делятся и на 3, и на 5. 

(На самом деле, этот вопрос подходит для собеседований, и, говорят, он позволяет отсеивать довольно большое число кандидатов. Поэтому, когда вы решите эту задачу, можете себя похвалить.) 

### 5.5 Таблица Умножения
Написать функцию, которая принимает в себя один аргумент (число) и печатает таблицу умножения на это число от 1 до 10

    printTable(3) 

    3 * 1 = 3
    3 * 2 = 6
    3 * 3 = 9
… (и так далее)

### 5.6 Треугольник
Напишите цикл, который за 7 вызовов console.log выводит такой треугольник:

    *
    **
    ***
    ****
    *****
    ******
    *******
    
Будет полезно знать, что длину строки можно узнать, приписав к переменной .length.

Когда справитесь, сделайте высоту треугольника переменной, чтобы можно было напечатать треугольники разной высоты, не только в 7 строк. 

### 5.7 Шахматная доска
Напишите программу, создающую строку, содержащую решётку 8х8, в которой линии разделяются символами новой строки. На каждой позиции либо пробел, либо #. В результате должна получиться шахматная доска. 

    # # # # 
     # # # # 
    # # # # 
     # # # # 
    # # # # 
     # # # # 
    # # # # 
     # # # # 

Когда справитесь, сделайте размер доски переменным, чтобы можно было создавать доски любого размера.

### Случайные кружочки:

Приложение рисует заданное количество кружков случайной окружности, цвета и позиции на экране. Количество кружков является аргументом функции. 

На картинке пример выполнения функции

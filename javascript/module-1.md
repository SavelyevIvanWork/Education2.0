# Vanilla JS
## Module 1

В первом модуле познакомимся с основами язака Java Script.

### Материалы для изучения:
- [Переменные](https://learn.javascript.ru/variables)
- [Типы данных](https://learn.javascript.ru/types)
- [Преобразование типов](https://learn.javascript.ru/type-conversions)
- [Базовые операторы, математика](https://learn.javascript.ru/operators)
- [Операторы сравнения](https://learn.javascript.ru/comparison)
- [Условное ветвление: if, '?'](https://learn.javascript.ru/ifelse)
- [Логические операторы](https://learn.javascript.ru/logical-operators)
- [Циклы while и for](https://learn.javascript.ru/while-for)
- [Конструкция "switch"](https://learn.javascript.ru/switch)
- [Функции](https://learn.javascript.ru/function-basics)
- [Function Expression](https://learn.javascript.ru/function-expressions)
- [Функции-стрелки, основы](https://learn.javascript.ru/arrow-functions-basics)
- [Особенности JavaScript](https://learn.javascript.ru/javascript-specials)
- [Объекты](https://learn.javascript.ru/object)
- [Массивы](https://learn.javascript.ru/array)
- [Методы массивов](https://learn.javascript.ru/array-methods)
- [Перебираемые объекты](https://learn.javascript.ru/iterable)
- [Object.keys, values, entries](https://learn.javascript.ru/keys-values-entries)

###Задачи

1.  Написать функцию, которая возвращает количество элементов массива, не используя 'array.length'.

___
2. В функцию передаются два параметра: массив и значение.
   По результату выполнения вернуть все элементы массива, которые равны второму параметру.

input:
```js script 
arraySearch([11, 57, 2, 110, 11, 94, 7], 11)
```
output:
```js script 
[11, 11]
```
___
3. В функцию передаются два параметра: массив и значение.
   По результату выполнения вернуть все элементы массива, которые больше второго параметра.


input:
```js script 
arraySearch([11, 57, 2, 110, 11, 94, 7], 67)
```
output:
```js script 
[110, 94]
```
---
4. В функцию передаем массив и значение.
   По результату выполнения вернуть все индексы элементов массива, которые меньше второго параметра.


input:
```js script 
arrayIndex([11, 57, 2, 110, 11, 94, 7], 30)
```
output:
```js script 
[0, 2, 4, 6]
```
___

5. В функцию передаем массив и значение.
   По результату выполнения вернуть номер последнего элемента массива, который равен второму параметру.


input:
```js script 
lastElementIndex([11, 3, 57, 2, 3, 110, 11, 3, 240, 94, 7], 3)
```
output:
```js script 
7
```
___

6. В функцию передаем два параметра: массив и значение.
   По результату выполнения вернуть все объекты массива, конкретное свойство 'make', которых равно второму параметру.

input:
```js script 
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, 'Ferrari')
```
output:
```js script 
    [
        {make: "Ferrari", model: "Dino", year: 1967}, 
        {make: "Ferrari", model: "Enzo", year: 2000}
    ]
```

___

7. В функцию передаем три параметра: массив и два значение.
   По результату выполнения вернуть все элементы массива, которые равны второму или третьему параметру.

input:
```js script 
arraySearch([11, 57, 2, 110, 11, 94, 7], 57, 7)
```
output:
```js script 
[67, 7]
```

___

8. В функцию передаем два параметра: массив и два значения.
   По результату выполнения вернуть все объекты, у которых свойство 'make' равно второму параметру или свойство 'year' равно третьему параметру.

input:
```js script 
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]
    arrayObjects(cars, "Porsche", 2000)
```
output:
```js script 
[
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]
```
___

9. В функцию передаем два параметра: массив и значение.
   По результату выполнения вернуть все объекты массива, свойство 'year', которых не равно второму параметру.

input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, 2000)
```
output:
```js script 
[
    {make: "Ford", model: "Mustang", year: 1969}, 
    {make: "Ferrari", model: "Dino", year: 1967}, 
    {make: "BMW", model: "Z8", year: 1999}, 
    {make: "Porsche", model: "911", year: 1981}
]
```
___

10. В функцию передаем три параметра: массив и значение.
    По результату выполнения вернуть true, если у всех объектов свойство 'make' равно второму параметру, а свойство 'year' равно третьему параметру.

input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, 'Ford', 1981)
```
output:
```js script 
false
```

input:
```js script
const cars = [
    {make: "Ferrari", model: "Maranello", year: 2000},
    {make: "Ferrari", model: "F1-2000", year: 2000},
    {make: "Ferrari", model: "Enzo", year: 2000},
]

arrayObjects(cars, 'Ferrari', 2000)
```
output:
```js script 
true
```
___

11. В функцию передаем три параметра: массив и значение.
    По результату выполнения вернуть true, если хотябы у одного объекта свойство 'make' равно второму параметру, а свойство 'year' равно третьему параметру.

input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, 'Ferrari', 2000)
```
output:
```js script 
true
```
___

12. В функцию передаем два параметра: массив и значение.
    По результату выполнения вывести true, если в массиве объектов есть свойство, значение которого равное второму параметру.

input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, "Enzo")
```
output:
```js script 
true
```
___

13. В функцию передаем два параметра: массив и название ключа.
    По результату выполнения вернуть массив значений по этому ключу всех объектов.

input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Mercedes-Benz", model: "W203", year: 2000},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars, "model")
```
output:
```js script 
[ 'Mustang', 'W203', 'Dino', 'Z8', 'Enzo', '911' ]
```
___

14. Найти максимальный/минимальный элемент в массиве.

input:
```js script
const arrNum = [11, 57, 2, 110, 11, 94, 7, 967, 8, 74, 601, -1032]

arraySearch(arrNum)
```
output:
```js script 
// {max: 967, min: -1032};
```
___

15. В функцию передаем массив с объектами.
    По результату выполнения вернуть объекты, значение свойства "year" которых максимальное и минимальное.


input:
```js script
const cars = [
    {make: "Ford", model: "Mustang", year: 1969},
    {make: "Ferrari", model: "Dino", year: 1967},
    {make: "BMW", model: "Z8", year: 1999},
    {make: "Mercedes-Benz", model: "GL", year: 2005},
    {make: "Ferrari", model: "Enzo", year: 2000},
    {make: "Porsche", model: "911", year: 1981}
]

arrayObjects(cars)
```
output:
```js script 
    [
        {make: "Ferrari", model: "Dino", year: 1967}, 
        {make: "Mercedes-Benz", model: "GL", year: 2005}
    ]
```
___

16. В функцию подается несколько массивов.
    Вернуть один массив со всеми элементами. Количество массивов может быть разное.

input:
```js script
concatenationArrays([11, 57, 2, 110, 11], ['crex', 'pex', 'fex'], [true, false])
```
output:
```js script 
[11, 57, 2, 110, 11, 'crex', 'pex', 'fex', true, false]
```
___

17. В функцию передаётся объект название свойства. Если свойство 'year' присутствует в объекте вернуть собщение "Exist", если отсутсвует вернуть сообщение "No exist".

input:
```js script
searchObjectKey({make: "Ford", model: "Mustang"}, 'year')
```
output:
```js script 
"No exist"
```

input:
```js script
searchObjectKey({make: "Ford", model: "Mustang", year: 1969}, 'year')
```
output:
```js script 
"Exist"
```
___ 

18. Нужно скопировать значения с одного массива в другой. В скопированном массиве изменить любой элемент и вывести 2 массива.

input:
```js script
copyingArray(["angel", "clown", "drum", "mandarin", "sturgeon"])
```
output:
```js script 
{
    arr1: [ 'angel', 'clown', 'drum', 'mandarin', 'sturgeon' ], 
    arr2: [ 'angel', 'clown', 'drum', 'sturgeon' ]
}
```
___

19. В функцию передаем массив.
    По результату выполнения вернуть массив, в котором отсутствуют ложные значения: false, null, undefined, 0, –0, NaN и "".

input:
```js script

const arr = [11, {make: "Ferrari", model: "Enzo", year: 2000}, false, 'flex', null, 0, 2, "", 110, NaN, 11, 94, -0]

copyingArray(arr)
```
output:
```js script 
[11, {make: "Ferrari", model: "Enzo", year: 2000}, 'flex', 2, 110, 11, 94]
```
___

20. Напишите функцию moveElement(arr, from, to), которая позволяет менять местами элементы из позиции from в позицию to.
    Если элемент с индексом from не найден вернуть сообщение: 'Item with index {from} not found!'

input:
```js script

const cars = ['BMW', 'Mercedes', 'Audi', 'Ferrari', 'ВАЗ', 'Peugeot', 'Hyundai']

moveElement(cars, 5, 3)
```
output:
```js script 
['BMW', 'Mercedes', 'Audi', 'Peugeot', 'Ferrari', 'ВАЗ', 'Hyundai']
```
___

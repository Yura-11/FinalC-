# Итоговая контрольная работа по основному блоку

## Задание :

1. Создать репозиторий на GitHub
2. Нарисовать блок-схему алгоритма (можно обойтись блок-схемой основной содержательной части, если вы выделяете её в отдельный метод)
3. Снабдить репозиторий оформленным текстовым описанием решения (файл README.md)
4. Написать программу, решающую поставленную задачу
5. Использовать контроль версий в работе над этим небольшим проектом (не должно быть так, что всё залито одним коммитом, как минимум этапы 2, 3, и 4 должны быть расположены в разных коммитах)

Задача: написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

Примеры:
[“Hello”, “2”, “world”, “:-)”] → [“2”, “:-)”]
[“1234”, “1567”, “-2”, “computer science”] → [“-2”]
[“Russia”, “Denmark”, “Kazan”] → []

# Решение

## 1. Создал репозиторий на GitHub.

Для того что бы создать репозиторий нам необходимо зайти на [сайт](https://github.com/), далее нажимаем на [New repository](https://github.com/new), и следуем дальнейшим инструкциям.

## 2. Рисуем блок-схему алгоритма.

Для этого мы используем программу [draw.io](https://app.diagrams.net/).
Получаем :

 ![блок-схему][/Алгоритм.png]

## 3. Решение программы выглядит следующим образом:

- Создаем массивы строк `array1`,`array2`,`array3` содержащие различные строки.

- Объявляем методы `SortArray1`,`SortArray2`,`SortArray3` для сортировки массива 

- В методах `SortArray1`,`SortArray2`,`SortArray3` создаются новые массивы `newArray1`,`newArray2`,`newArray3` с тем же размером, что и входные массивы `array1`,`array2`,`array3`.

- Объявляем переменные `count`, которые будут использоваться для отслеживания количества элементов, добавленных в новые массивы.

- Проходимся циклом по всем элементам массивов `array1`,`array2`,`array3`:
если длина текущей строки меньше или равна 3 символам, то эта строка копируется в новые массивы `newArray1`,`newArray2`,`newArray3` соответсвено на позиции `count`, и значения `count` увеличивается на 1.

- Возвращаем новые массивы `newArray1`,`newArray2`,`newArray3` которые содержат только строки с длиной не более 3 символов.
- Далее с помощью команды `Console.Write` выводим начальные массивы и конечные массивы, содержащий меньше или равно 3 символам строки.

[def]: <Алгоритм .png>
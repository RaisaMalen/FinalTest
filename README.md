## Задача:
Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

## Решение: 
1. Для начала необходимо задать первоначальный массив строк **firstArray**. В данном случае задам его на старте выполнения алгоритма.
2. Далее объявляю второй - пустой массив **secondArray**, такой же длины, как и первый массив. В этот массив будут вноситься строки, удовлетворяющие условию задачи.
3. Теперь описываю метод **CreateSecondArray**, в котором будет цикл **for** соизмеримый длине первоначального массива **firstArray** - этот цикл будет выполняться до тех пор, пока не будут проверены удовлетворению условию задачи все строки первоначального массива. Соответственно, при каждом возвращениие программы к циклу **for**, индекс (**i**) будет увеличиваться на единицу, до тех пор пока **i** меньше длины первоначального массива. Внутри цикла будет проверяться условие задачи - поиск строк в первоначальном массиве, длина которых меньше, либо равна трем символам. Если проверяемая строка первоначального заданного массива удовлетворяет условию задачи - ее длина равна либо меньше трех символов, то тогда эта строка будет записываться в соответствующий элемент (**count** элемент) второго массива **secondArray**. Переменная **count** создана, чтобы поочередно перемещать нужные строки из первоначального массива во второй и без пробелов. После положительной проверки условия - перемещения строки, удовлетворяющей условию задачи во второй массив, переменная **count** увеличивается на единицу и программа возвращается к циклу **for**. Если проверяемая строка первоначального заданного массива не удовлетворяет условию задачи - программа возвращается к циклу **for**.
4. Далее создаем метод вывода заданного массива на консоль **PrintArray**. В этом методе также используется цикл **for** - пока индекс **i** элемента заданного массив меньше его длины, элемент с указанным индексом будет выводиться в консоль. Элементы массива будут выведены через пробел.
5. Обращаюсь к методу **CreateSecondArray**.
6. Обращаюсь к методу **PrintArray**.

# Dynamic Programming
## A. Необычные числа

ограничение по времени на тест: 1 секунда

ограничение по памяти на тест: 64 мегабайта

ввод: стандартный ввод

вывод: стандартный вывод

Большинство чисел слишком обычные, чтобы давать на них задачи. Вот, например, Ивану дали задачу: для данного натурального числа проверить, правда ли, что среди **всех целых чисел** есть
ровно 4, на которые оно делится. Он написал программу, но Саша решила, что у него и так многовато баллов по алгоритмам, и стерла часть его кода.

```c++
#include <iostream>
using namespace std;

bool is_unusual(int n) {
... кажется, здесь должен быть код ...
}

int main() {
  int n;
  cin >> n;
  cout << is_unusual(n) ? "True" : "False";
}
```

Помогите Ивану восстановить стертую часть!

### Входные данные:
Вводится одно число n $(2 \leq n \leq 10^{12})$

### Выходные данные:
Надо вывести `True`, если число удовлетворяет условию, и `False`, если нет.

### Пример

**входные данные**
```c++
2
```
**выходные данные**
```c++
True
```
**входные данные**
```c++
10
```
**выходные данные**
```c++
False
```



## B. Решето Эратосфена

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 64 мегабайта

ввод: стандартный ввод

вывод: стандартный вывод

По введенным числам A и B вывести все простые числа в интервале от A до B включительно.

### Входные данные:
В единственной строке вводятся два числа 1 ≤ A ≤ B ≤ 500000

### Выходные данные:
Вывести в одну строку все простые числа в интервале от A до B включительно

### Примеры

**входные данные**
```c++
2 2
```
**выходные данные**
```c++
2
```
**входные данные**
```c++
1 100
```
**выходные данные**
```c++
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97
```


## C. Массовая проверка простоты

ограничение по времени на тест: 1.5 секунд

ограничение по памяти на тест: 512 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Целое число p≥2 является простым, если у него нет делителей кроме 1 и p. Необходимо для всех чисел во входном файле проверить простые они или нет.

### Входные данные:
В первой строке задано число n (2≤n≤500000). В следующих n строках заданы числа ai $(2\leq a_i \leq 2\cdot 10^7)$, которые нужно проверить на простоту

### Выходные данные:
Для каждого числа во входном файле выведите на отдельной строке `«YES»` или `«NO»` в зависимости от того, простое оно или нет.

### Примеры

**входные данные**
```c++
4
60
14
3
55
```

**выходные данные**
```c++
NO
NO
YES
NO
```


## D. Разложение на множители

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Дано число. Требуется разложить его на простые множители.

### Входные данные:
Вводится число n $(2 \leq  n \leq 10^9)$.

 ### Выходные данные:
 Выведите через пробел разложение на простые множители в порядке неубывания множителей.

 ### Примеры

**входные данные**
```c++
17
```

**выходные данные**
```c++
17
```
**входные данные**
```c++
60
```

**выходные данные**
```c++
2 2 3 5
```


## E. Массовое разложение на множители

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Дано много чисел. Требуется разложить их все на простые множители.

### Входные данные:
В первой строке задано число n (2≤n≤300000). В следующих n строках заданы числа $a_i$ $(2 \leq a_i \leq 2\cdot 10^6)$, которые нужно разложить на множители.

### Выходные данные:
Для каждого числа выведите в отдельной строке разложение на простые множители в порядке возрастания множителей.

### Пример

**входные данные**
```c++
4
60
14
3
55
```

**выходные данные**
```c++
2 2 3 5 
2 7 
3 
5 11 
```


## F. МегаНОД

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 64 мегабайта

ввод: стандартный ввод

вывод: стандартный вывод

Найдите НОД N заданных чисел.

### Входные данные:
Первая строка входного файла содержит натуральное число N (1  ≤  N  ≤  1 000) — количество чисел. Во второй строке заданы N чисел, не превышающие по модулю $10^9$.

### Выходные данные:
Выведите НОД N чисел.

### Пример

**входные данные**
```c++
2
90 35
```
**выходные данные**
```c++
5
```


## G. Шестеренки

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Даны две сцепленные шестерёнки. У одной шестерёнки N зубцов, у другой — K. Требуется найти, какое минимальное число поворотов на один зубчик требуется сделать, чтобы шестерёнки вернулись в исходное состояние.

### Входные данные:
В единственной строке — два числа, N и K. $1 \leq N, K \leq 10^7$.

### Выходные данные:
Выведите искомое количество зубчиков.

### Примеры 

**входные данные**
```c++
2 3
```
**выходные данные**
```c++
6
```
**входные данные**
```c++
6 21
```
**выходные данные**
```c++
42
```


## H. Сумма дробей

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Обыкновенная дробь называется несократимой, если её числитель и знаменатель взаимно просты. Даны две обыкновенные несократимые дроби $\frac{a}{b}$ и $\frac{c}{d}$. Найдите их сумму также в виде обыкновенной несократимой дроби.

### Входные данные:
В первой строке даны четыре числа a, b, c и d ( - 1000 ≤ a, c ≤ 1000, 1 ≤ b, d ≤ 1000).

### Выходные данные:
В единственной строке выведите два числа через пробел — числитель и знаменатель ответа. При этом знаменатель дроби всегда должен быть положительным.

### Примеры 

**входные данные**
```c++
1 2 3 4
```
**выходные данные**
```c++
5 4
```
**входные данные**
```c++
-1 6 1 6
```
**выходные данные**
```c++
0 1
```


## J. НОД подмножества

ограничение по времени на тест: 2 секунды

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Сегодня на уроке математики шестиклассник Петя изучил понятие наибольшего общего делителя. Петя тут же решил применить полученные знания на практике.

Петя выписал на листке бумаги n чисел $a_1, ..., a_n$ — номера домов, в которых живут его друзья. Теперь он хочет выбрать такое подмножество этих чисел, чтобы их наибольший общий делитель был равен его любимому числу d.

Помогите Пете выбрать из выписанных чисел искомое подмножество.

### Входные данные:
Первая строка входного файла содержит два целых числа n и d $(1 \leq n \leq 1000, 1 \leq d \leq 10^9)$. Вторая строка содержит n целых чисел: $a_1, a_2, ..., a_n$ $(1 \leq a_i \leq 10^9)$.

### Выходные данные:
Если существует искомое подмножество, выведите на первой строке выходного файла число k — количество чисел в нем. На второй строке выведите числа, входящие в это подмножество.

Если решения не существует, выведите на первой строке выходного файла число  - 1.

Если возможных ответов несколько, выведите любой из них.

### Примеры

**входные данные**
```c++
4 3
6 8 12 9
```
**выходные данные**
```c++
3
6 12 9 
```
**входные данные**
```c++
3 3
2 4 8
```
**выходные данные**
```c++
-1
```



## K. Китайская теорема

ограничение по времени на тест: 1 секунда

ограничение по памяти на тест: 256 мегабайт

ввод: стандартный ввод

вывод: стандартный вывод

Решите в целых числах систему уравнений

$x \equiv a\mod n$ & $x \equiv b\mod m$,

где n и m взаимно просты. Среди решений следует выбрать наименьшее неотрицательное число.

### Входные данные:
Первая строка входных данных содержит число N, $1\leq N\leq 10^4$, — количество тестов, для которых нужно решить задачу.

Следующие N строк содержат по четыре целых числа $a_i$, $b_i$, $n_i$ и $m_i$ $(1 \leq n_i , m_i \leq 10^9, 0 \leq a_i < n_i, 0 \leq b_i < m_i)$.

### Выходные данные:
Для каждого из тестов выведите искомое наименьшее неотрицательное число $x_i$.

### Пример

**входные данные**
```c++
2
1 0 2 3
3 2 5 9
```
**выходные данные**
```c++
3
38
```

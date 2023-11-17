# InfoBase_and_Database
Папка МДК 12.01 со всеми работами: https://drive.google.com/drive/folders/1-GTu7U7AbG-MKZmo8Gm2osoFvmRMKcFF

09.10.23 09.10.23 конспект по БД и СУБД : https://docs.google.com/document/d/1xAeckTTQ2eGfsvaHNObcDQ0Vt_wrFqWZf3Vxa7mS4Nk/edit?usp=sharing 

09.10.23 ответы на вопросы: https://docs.google.com/document/d/1K5K8mf7uaDLJICscSgbysArxUHgfMiMCjgLJ3SiKVMc/edit?usp=sharing

26.10.23.sait: https:[//1top4ik1.github.io/Testsait/](https://1top4ik1.github.io/sait/)https://1top4ik1.github.io/sait/

06.10.23  конспект по python: https://docs.google.com/document/d/1jwE27z3xjXLeQwOyNmmtipD2Py-yFO6kdnxzHLIh4X0/edit?usp=sharing

06.10.23 задания по python: https://docs.google.com/document/d/1e3rYkr41QjWwjdwq2Z8iRcH129zMzSL19tTgGoB9wTY/edit?usp=sharing

bluefish and pycharm: https://docs.google.com/document/d/18cETZRFiMzgVvR5ri8V8NxBINjTF0vfxVZSQWs0koKU/edit?usp=sharing


Наименьшее из  2 чисел

a = int(input("Введите первое число: "))
b = int(input("Введите второе число: "))

if a>b:
    print("Наименьшее число: ", b)
else :
    print("Наименьшее число: ", a)


Наименьшее из 4 чисел

def find_minimum(a, b, c, d):
    min_ab = min(a, b)
    min_cd = min(c, d)
    return min(min_ab, min_cd)

num1 = int(input("Введите первое число: "))
num2 = int(input("Введите второе число: "))
num3 = int(input("Введите третье число: "))
num4 = int(input("Введите четвертое число: "))

result = find_minimum(num1, num2, num3, num4)
print("Наименьшее число: ", result)



Возрастная группа


def determine_age_group(age):
    if age <= 13:
        return "детство"
    elif 14 <= age <= 24:
        return "молодость"
    elif 25 <= age <= 59:
        return "зрелость"
    else:
        return "старость"

user_age = int(input("Введите возраст пользователя: "))
age_group = determine_age_group(user_age)
print("Возрастная группа: ", age_group)




Только +



def sum_of_positive_numbers(num1, num2, num3):
    sum_positive = 0
    if num1 > 0:
        sum_positive += num1
    if num2 > 0:
        sum_positive += num2
    if num3 > 0:
        sum_positive += num3
    return sum_positive

number1 = int(input("Введите первое число: "))
number2 = int(input("Введите второе число: "))
number3 = int(input("Введите третье число: "))

result = sum_of_positive_numbers(number1, number2, number3)
print("Сумма положительных чисел: ", result)



Красивое число



def is_beautiful_number(number):
    if 1000 <= number <= 9999 and (number % 7 == 0 or number % 17 == 0):
        return "YES"
    else:
        return "NO"

user_number = int(input("Введите четырехзначное число: "))
result = is_beautiful_number(user_number)
print("Результат: ", result)


Неравенство треугольника


def is_triangle(a, b, c):
    if a + b > c and a + c > b and b + c > a:
        return "YES"
    else:
        return "NO"


side1 = int(input("Введите длину первой стороны: "))
side2 = int(input("Введите длину второй стороны: "))
side3 = int(input("Введите длину третьей стороны: "))

result = is_triangle(side1, side2, side3)
print("Результат: ", result)




Високосный год


def is_leap_year(year):
    if year % 4 == 0 and year % 100 != 0 or year % 400 == 0:
        return "YES"
    else:
        return "NO"

user_year = int(input("Введите год: "))
result = is_leap_year(user_year)
print("Результат: ", result)




Ход ладьи


def can_rook_move(x1, y1, x2, y2):
    if x1 == y1 or y1 == x1:
        return "YES"
    else:
        return "NO"

x1 = int(input("Введите номер столбца для первой клетки: "))
y1 = int(input("Введите номер строки для первой клетки: "))
x2 = int(input("Введите номер столбца для второй клетки: "))
y2 = int(input("Введите номер строки для второй клетки: "))

result = can_rook_move(x1, y1, x2, y2)
print("Результат: ", result)




Ход короля



def can_king_move(x1, y1, x2, y2):
    if abs(x1 - x2) <= 1 and abs(y1 - y2) <= 1:
        return "YES"
    else:
        return "NO"

x1 = int(input("Введите номер столбца для первой клетки: "))
y1 = int(input("Введите номер строки для первой клетки: "))
x2 = int(input("Введите номер столбца для второй клетки: "))
y2 = int(input("Введите номер строки для второй клетки: "))

result = can_king_move(x1, y1, x2, y2)
print("Результат: ", result)









Модуль 2

Гонка спидстеров

v_zoom = int(input())
v_flash = int(input())

if v_zoom > v_flash:
    print("NO")
elif v_flash > v_zoom:
    print("YES")
else:
    print("Don't know")



    Вид треугольника



a = int(input("Введите длину первой стороны: "))
b = int(input("Введите длину второй стороны: "))
c = int(input("Введите длину третьей стороны: "))

if a + b <= c or a + c <= b or b + c <= a:
    print("Треугольник не существует")
elif a == b == c:
    print("Равносторонний")
elif a == b or b == c or a == c:
    print("Равнобедренный")
else:
    print("Разносторонний")




    Среднее число


    a = int(input("Введите первое число: "))
b = int(input("Введите второе число: "))
c = int(input("Введите третье число: "))

if a > b:
    if b > c:
        print(b)
    elif a > c:
        print(c)
    else:
        print(a)
else:
    if a > c:
        print(a)
    elif b > c:
        print(c)
    else:
        print(b)





        Количество дней



        month = int(input("Введите порядковый номер месяца: "))

if month in [1, 3, 5, 7, 8, 10, 12]:
    print("В этом месяце 31 день")
elif month in [4, 6, 9, 11]:
    print("В этом месяце 30 дней")
elif month == 2:
    print("В этом месяце 28 дней")
else:
    print("Ошибка: введите число от 1 до




    Церемнония взвешивания


    weight = int(input("Введите вес боксера: "))

if weight < 60:
    print("Легкий вес")
elif weight < 64:
    print("Первый полусредний вес")
elif weight < 69:
    print("Полусредний вес")
else:
    print("Весовая категория не определена")








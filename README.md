# Урок 1. знакомство с Python
# Задание 1.
# Задание 1.1: Поработайте с переменными, создайте несколько, выведите на экран.
#a = 10
#b = 15
#egor = 20
#egor_podkorytov = 25
#c = egor + egor_podkorytov + b * a
#print(c)

# Задание 1.2: запросите у пользователя несколько чисел и строк и сохраните в переменные, выведите на экран.
#a = int(input("Введите сколько Вам лет:  "))
#print("Мне " + str(a) + " лет")
#b = input("Введите как Вас зовут:   ")
#print("Привет, меня зовут" + b + "!")


# Задание 2. Пользователь вводит время в секундах. Переведите время в часы, минуты и секунды и выведите в формате чч:мм:сс.
# Используйте форматирование строк.

#a = int(input("Введите время в секундах:  "))
#Часы
#b = a // 3600
#Минуты
#c = (a - b * 3600) // 60
#Секунды
#d = (a - b * 3600) - c * 60

#print(f"Время (чч:мм:сс):  ", str(b) + ":" + str(c) + ":" + str(d))  # Когда я хочу вывести: print("Время (чч:мм:сс): "), a + ":" + b + ":" + c) - он выдаёт ошибку, поэтому всем переменным я задаю тип строки (ТОЛЬКО В ПРИНТЕ).
#print("%-5s %-10s %-15s" % ('str(b)', 'str(c)', 'str(d)'))
# у меня не получается ни с одним форматированием, я не понимаю куда что вставлять... Строчка 30 вообще не то выдаёт




# Задание 3. Узнайте у пользователя число n. Найдите сумму чисел n + nn + nnn. Например, пользователь ввёл число 3.
# Считаем 3 + 33 + 333 = 369.

#a = int(input("Давайте найдём сумму чисел n + nn + nnn. Введите число n:  "))
#b = (a + int(str(a) + str(a)) + int(str(a) + str(a) + str(a)))

#print("Считаем: ", a, '+', int(str(a) + str(a)), "+", int(str(a) + str(a) + str(a)), '=', b)


# Задание 4. Пользователь вводит целое положительное число. Найдите самую большую цифру в числе.
# Для решения используйте цикл while и арифметические операции.

#a = int(input("Введите целое положительное число и я найду самую большую цифру в числе:  "))

#max_number = a % 10
#while a >= 1:
   # a = a // 10
   # if a % 10 > max_number:
   #     max_number = a % 10
   # if a > 9:
   #     continue
   # else:
   #     print("Максимальнае цифра в числе ", max_number)
   # break
# Весь код я скопировал с готового решения, и при этом я ничего не понял, особенно строчку 50.

#Задание5. Запросите у пользователя значения выручки и издержек фирмы.
#Определите, с каким финансовым результатом работает фирма (прибыль — выручка больше издержек, или убыток — издержки больше выручки).
#Выведите соответствующее сообщение. Если фирма отработала с прибылью, вычислите рентабельность выручки (соотношение прибыли к выручке).
#Далее запросите численность сотрудников фирмы и определите прибыль фирмы в расчете на одного сотрудника.

#a = int(input("Введите значения выручки фирмы:  "))
#b = int(input("Введите значения издержек фирмы:  "))
#if a > b:
  #  print("Фирма работает в прибыль", "Рентабельность выручки: ", (a-b) / b)
  #  c = int(input("Введите численность сотрудников фирмы:  "))
  #  print("Прибыль фирмы в расчете на одного сотрудника: ", (a - b) / c)
#else:
  #  print("Фирма работает в убыток")

#Задание6. Спортсмен занимается ежедневными пробежками. В первый день его результат составил a километров.
#Каждый день спортсмен увеличивал результат на 10 % относительно предыдущего.
#Требуется определить номер дня, на который общий результат спортсмена составить не менее b километров.
#Программа должна принимать значения параметров a и b и выводить одно натуральное число — номер дня.

#a = int(input("ведите сколько км пробежал спортсмен в первый день: "))
#b = int(input("Введите сколько км нужно пробежать спортсмену: "))
#day = 1   #всего дней
#km = a    #всего км
#while km <= b:
#        a = a + 0.1 * a
#        day += 1
#        km = km + a

#print(f"Результат:\n1-й день: ")
#print(f"%.d-й день: " % day, a)
#print(f"Вы достигнете требуемых показателей на %.d день" % day)
#print(f"Ответ: на %.d-й день спортсмен достиг результата — не менее" % day, b, "км")
# не получается, уже голову сломал, взял из готовых решений но строка 86 неправильная

# -18.8.19-
Необходимо написать программу, которая будет подсчитывать общую стоимость билетов
all_price = 0
tickets = int(input('Укажите количество билетов '))
for i in range(tickets):
   age = int(input("Укажите возраст посетителя "))
   if age < 18:
      print(("бесплатно"))
   elif 18 <= age < 25:
      all_price += 990
      print("990 руб.")
   else:
      all_price += 1390
      print("полная стоимость 1390 руб.")
if tickets > 3:
   all_price = all_price - ((all_price / 100) * 10)
   print("Сумма к оплате", all_price, "руб.")
else:
   print("Сумма к оплате", all_price, "руб.")

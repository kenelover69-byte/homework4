# Введення списку з 10 чисел з клавіатури
print("Введіть 10 цілих чисел:")
numbers = []
for i in range(10):
  num = int(input(f"Елемент {i + 1}: "))
  numbers.append(num)

found = False
first_index = -1

# Перевірка елементів списку
for index, num in enumerate(numbers):
  # Перевіряємо, чи є число тризначним (враховуємо і додатні, і від'ємні числа через abs)
  abs_num = abs(num)
  if 100 <= abs_num <= 999:
    # Обчислюємо суму цифр числа
    digit_sum = sum(int(digit) for digit in str(abs_num))

    # Перевіряємо, чи кратне число сумі своїх цифр
    if num % digit_sum == 0:
      found = True
      first_index = (
          index  # Запам'ятовуємо індекс першого такого елемента та виходимо
      )
      break

# Виведення результату
if found:
  print("\nТак")
  print(f"Індекс першого такого елемента: {first_index}")
else:
  print("\nНі, серед введених чисел немає тризначних, які кратні сумі своїх цифр.")

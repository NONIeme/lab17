# Лабораторна робота №17: Генератори у Python

## Мета роботи
Метою даної лабораторної роботи є розробка різних генераторів для виконання широкого спектру задач, таких як обхід дерев, генерація числових послідовностей, робота з файлами та інше.

### Опис завдань
1. **Task 1**: Створення генератора для ітерації по списку чисел.
2. **Task 2**: Генератор, що повертає парні числа з заданого діапазону.
3. **Task 3**: Генератор, що повертає непарні числа з заданого діапазону.
4. **Task 4**: Генератор, що виробляє числа Фібоначчі.
5. **Task 5**: Генератор, що повертає прості числа до заданої межі.
6. **Task 6**: Генератор для проходження бінарного дерева у префіксному порядку.
7. **Task 7**: Генератор для проходження бінарного дерева у інфіксному порядку.
8. **Task 8**: Генератор для проходження бінарного дерева у постфіксному порядку.
9. **Task 9**: Генератор для обходу графа за алгоритмом глибини (DFS).
10. **Task 10**: Генератор для обходу графа за алгоритмом ширини (BFS).
11. **Task 11**: Генератор, що повертає ключі словника.
12. **Task 12**: Генератор, що повертає значення словника.
13. **Task 13**: Генератор, що повертає пари ключ-значення зі словника.
14. **Task 14**: Генератор, що повертає рядки з файлу.
15. **Task 15**: Генератор, що повертає слова з текстового файлу.
16. **Task 16**: Генератор, що повертає символи зі строки.
17. **Task 17**: Генератор, що повертає унікальні елементи зі списку.
18. **Task 18**: Генератор, що повертає елементи списку у зворотному порядку.
19. **Task 19**: Генератор, що повертає декартів добуток двох списків.
20. **Task 20**: Генератор, що повертає перестановки зі списку.
21. **Task 21**: Генератор, що повертає комбінації зі списку елементів.
22. **Task 22**: Генератор для ітерації по списку кортежів.
23. **Task 23**: Генератор, що повертає елементи з кількох списків паралельно.
24. **Task 24**: Генератор, що повертає елементи з вкладеного списку (розгортання списку).
25. **Task 25**: Генератор, що повертає елементи з вкладеного словника.
26. **Task 26**: Генератор, що повертає степені числа 2 до заданого числа.
27. **Task 27**: Генератор, що повертає степені заданої основи до певної межі.
28. **Task 28**: Генератор, що повертає квадрати чисел у заданому діапазоні.
29. **Task 29**: Генератор, що повертає куби чисел у заданому діапазоні.
30. **Task 30**: Генератор, що повертає факторіали чисел до заданої межі.
31. **Task 31**: Генератор, що повертає числа з послідовності Коллатца.
32. **Task 32**: Генератор, що повертає числа у геометричній прогресії.
33. **Task 33**: Генератор, що повертає числа в арифметичній прогресії.
34. **Task 34**: Генератор, що повертає поточну суму списку чисел.
35. **Task 35**: Генератор, що повертає поточний добуток списку чисел.

## Виконання роботи
### Кроки виконання
1. Кожна лабораторна робота повинна бути завантажена в окрему папку на GitHub.
2. Назва папки повинна містити номер лабораторної роботи (наприклад, `lab17`).
3. В кожній папці повинні бути присутні наступні файли:
   - Основний код програми (`student_main.py`).
   - README файл з детальним поясненням.

### Структура проекту
lab8
- ├── student_main.py
- ├── README.md

### Опис файлів
- **student_main.py**: Основний код програми, що містить п'ять завдань для роботи з JSON файлами.
- **README.md**: Файл з детальним поясненням.

### Приклади використання
```python
# Task 1: Приклад використання генератора для ітерації по списку чисел
numbers = [1, 2, 3, 4, 5]
gen = number_generator(numbers)
print(next(gen))  # 1
print(next(gen))  # 2

# Task 2: Приклад використання генератора парних чисел
even_gen = even_number_generator(1, 10)
print(list(even_gen))  # [2, 4, 6, 8, 10]

# Task 3: Приклад використання генератора непарних чисел
odd_gen = odd_number_generator(1, 10)
print(list(odd_gen))  # [1, 3, 5, 7, 9]

# Task 4: Приклад використання генератора чисел Фібоначчі
fib_gen = fibonacci_generator()
print(next(fib_gen))  # 0
print(next(fib_gen))  # 1
print(next(fib_gen))  # 1
print(next(fib_gen))  # 2

# Task 5: Приклад використання генератора простих чисел
prime_gen = prime_number_generator(10)
print(list(prime_gen))  # [2, 3, 5, 7]

# Task 6: Приклад використання генератора для проходження бінарного дерева у префіксному порядку
root = TreeNode(1, TreeNode(2), TreeNode(3))
pre_order_gen = pre_order_traversal(root)
print(list(pre_order_gen))  # [1, 2, 3]

# Task 7: Приклад використання генератора для проходження бінарного дерева у інфіксному порядку
in_order_gen = in_order_traversal(root)
print(list(in_order_gen))  # [2, 1, 3]

# Task 8: Приклад використання генератора для проходження бінарного дерева у постфіксному порядку
post_order_gen = post_order_traversal(root)
print(list(post_order_gen))  # [2, 3, 1]

# Task 9: Приклад використання генератора для обходу графа за алгоритмом глибини (DFS)
graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}
dfs_gen = dfs_traversal(graph, 'A')
print(list(dfs_gen))  # ['A', 'B', 'D', 'E', 'F', 'C']

# Task 10: Приклад використання генератора для обходу графа за алгоритмом ширини (BFS)
bfs_gen = bfs_traversal(graph, 'A')
print(list(bfs_gen))  # ['A', 'B', 'C', 'D', 'E', 'F']

# Task 11: Приклад використання генератора, що повертає ключі словника
d = {'a': 1, 'b': 2, 'c': 3}
keys_gen = dict_keys_generator(d)
print(list(keys_gen))  # ['a', 'b', 'c']

# Task 12: Приклад використання генератора, що повертає значення словника
values_gen = dict_values_generator(d)
print(list(values_gen))  # [1, 2, 3]

# Task 13: Приклад використання генератора, що повертає пари ключ-значення зі словника
items_gen = dict_items_generator(d)
print(list(items_gen))  # [('a', 1), ('b', 2), ('c', 3)]

# Task 14: Приклад використання генератора, що повертає рядки з файлу
# Створимо тестовий файл для прикладу
with open('test.txt', 'w') as f:
    f.write("First line\nSecond line\nThird line")

lines_gen = file_lines_generator('test.txt')
print(list(lines_gen))  # ['First line', 'Second line', 'Third line']

# Task 15: Приклад використання генератора, що повертає слова з текстового файлу
words_gen = file_words_generator('test.txt')
print(list(words_gen))  # ['First', 'line', 'Second', 'line', 'Third', 'line']

# Task 16: Приклад використання генератора, що повертає символи зі строки
chars_gen = string_chars_generator("hello")
print(list(chars_gen))  # ['h', 'e', 'l', 'l', 'o']

# Task 17: Приклад використання генератора, що повертає унікальні елементи зі списку
unique_gen = unique_elements_generator([1, 2, 2, 3, 3, 3, 4])
print(list(unique_gen))  # [1, 2, 3, 4]

# Task 18: Приклад використання генератора, що повертає елементи списку у зворотному порядку
reverse_gen = reverse_list_generator([1, 2, 3, 4, 5])
print(list(reverse_gen))  # [5, 4, 3, 2, 1]

# Task 19: Приклад використання генератора, що повертає декартів добуток двох списків
cartesian_gen = cartesian_product_generator([1, 2], ['a', 'b'])
print(list(cartesian_gen))  # [(1, 'a'), (1, 'b'), (2, 'a'), (2, 'b')]

# Task 20: Приклад використання генератора, що повертає перестановки зі списку
permutations_gen = permutations_generator([1, 2, 3])
print(list(permutations_gen))  # [(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]

# Task 21: Приклад використання генератора, що повертає комбінації зі списку елементів
combinations_gen = combinations_generator([1, 2, 3], 2)
print(list(combinations_gen))  # [(1, 2), (1, 3), (2, 3)]

# Task 22: Приклад використання генератора для ітерації по списку кортежів
tuples_gen = tuple_list_generator([(1, 2), (3, 4), (5, 6)])
print(list(tuples_gen))  # [(1, 2), (3, 4), (5, 6)]

# Task 23: Приклад використання генератора, що повертає елементи з кількох списків паралельно
parallel_gen = parallel_lists_generator([1, 2, 3], ['a', 'b', 'c'])
print(list(parallel_gen))  # [(1, 'a'), (2, 'b'), (3, 'c')]

# Task 24: Приклад використання генератора, що повертає елементи з вкладеного списку (розгортання списку)
nested_list = [1, [2, 3], [4, [5, 6]], 7]
flatten_gen = flatten_list_generator(nested_list)
print(list(flatten_gen))  # [1, 2, 3, 4, 5, 6, 7]

# Task 25: Приклад використання генератора, що повертає елементи з вкладеного словника
nested_dict = {'a': 1, 'b': {'c': 2, 'd': 3}, 'e': 4}
nested_dict_gen = nested_dict_generator(nested_dict)
print(list(nested_dict_gen))  # [('a', 1), ('c', 2), ('d', 3), ('e', 4)]

# Task 26: Приклад використання генератора, що повертає степені числа 2 до заданого числа
powers_of_two_gen = powers_of_two_generator(4)
print(list(powers_of_two_gen))  # [1, 2, 4, 8, 16]

# Task 27: Приклад використання генератора, що повертає степені заданої основи до певної межі
powers_of_base_gen = powers_of_base_generator(3, 100)
print(list(powers_of_base_gen))  # [1, 3, 9, 27, 81]

# Task 28: Приклад використання генератора, що повертає квадрати чисел у заданому діапазоні
squares_gen = squares_generator(1, 5)
print(list(squares_gen))  # [1, 4, 9, 16, 25]

# Task 29: Приклад використання генератора, що повертає куби чисел у заданому діапазоні
cubes_gen = cubes_generator(1, 5)
print(list(cubes_gen))  # [1, 8, 27, 64, 125]

# Task 30: Приклад використання генератора, що повертає факторіали чисел до заданої межі
factorials_gen = factorials_generator(5)
print(list(factorials_gen))  # [1, 1, 2, 6, 24, 120]

# Task 31: Приклад використання генератора, що повертає числа з послідовності Коллатца
collatz_gen = collatz_sequence_generator(7)
print(list(collatz_gen))  # [7, 22, 11, 34, 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1]

# Task 32: Приклад використання генератора, що повертає числа у геометричній прогресії
geometric_gen = geometric_progression_generator(2, 3, 100)
print(list(geometric_gen))  # [2, 6, 18, 54]

# Task 33: Приклад використання генератора, що повертає числа в арифметичній прогресії
arithmetic_gen = arithmetic_progression_generator(1, 3, 10)
print(list(arithmetic_gen))  # [1, 4, 7, 10]

# Task 34: Приклад використання генератора, що повертає поточну суму списку чисел
running_sum_gen = running_sum_generator([1, 2, 3, 4])
print(list(running_sum_gen))  # [1, 3, 6, 10]

# Task 35: Приклад використання генератора, що повертає поточний добуток списку чисел
running_product_gen = running_product_generator([1, 2, 3, 4])
print(list(running_product_gen))  # [1, 2, 6, 24]
```
## Результати
В процесі роботи були успішно реалізовані всі необхідні генератори для виконання різних задач. Тестування функцій підтвердило їх коректність та відповідність вимогам.

## Висновки
Мета роботи була досягнута. Було реалізовано різні генератори для виконання широкого спектру задач. Всі завдання були виконані успішно, проблеми не виникли.

### Інструкції з запуску

Вимоги до середовища
- **Python версії 3.x
- **Необхідні бібліотеки: permutations, combinations

Команда для запуску
```
python main.py
```

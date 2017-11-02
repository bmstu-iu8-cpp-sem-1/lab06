## Лабораторная работа 6

### Инструкция
Каждое задание должно быть выполненно в отдельном `.cpp` файле.
Прототипы функции должны быть вынесены в соответствующие `.hpp` файлы.
Все реализованные функции необходимо вызвать в фунции `main` в файле [lab06](lab06.cpp)
Все `.cpp` файлы добавить в `CMakeLists.txt`

### Задание
1. Реализуйте функцию поиска элемента в диапазоне от `first` до `end`. Требуется вернуть итератор указывающий на найденный элемент. Если элемента нет, верните итератор `last`.
Прототип функции:
```cpp
std::vector<int>::iterator find(std::vector<int>::iterator first, std::vector<int>::iterator last, int el);
```
Пример использования функции:
```cpp
std::vector<int> v = {6, 8, 1, 2, 3, 4, 5};
std::vector<int>::iterator it = find(v.begin(), v.end(), 2);
```

2. Реализуйте функцию поиска элемента в диапозоне от `first` до `end`. **Известно**, что значения в диапазоне отсортированный. Требуется вернуть итератор указывающий на найденный элемент. Если элемента нет, верните итератор `last`.
Прототип функции:
```cpp
std::vector<int>::iterator findInSorted(std::vector<int>::iterator first, std::vector<int>::iterator last, int el);
```
Пример использования функции:
```cpp
std::vector<int> v = {1, 2, 3, 4, 5};
std::vector<int>::iterator it = findInSorted(v.begin(), v.end(), 2);
```

3. Реализуйте функцию, которая считает количество слов в предложении. Слова разделяются или `' '`, или `','` или `'.'`.
Прототип функции необходимо выбрать самостоятельно.

4. Реализуйте функцию, которая подсчитает количество вхождения различных слов в предложении. Слова разделяются или `' '`, или `','` или `'.'`. Функция должна возвращать `std::map<std::string, int>`
Пример использования функции:
```cpp
std::map<std::string, int> words = func("can you can");
// words["can"] == 2
// words["you"] == 1
```

5. Реализуйте функцию, которая вернет уникальные слова в предложении. Слова разделяются или `' '`, или `','` или `'.'`. Подберите подходящий прототип функции и структуры данных.

6. Реализуйте функцию, которая подсчитает количество различных слов в предложении. Слова разделяются или `' '`, или `','` или `'.'`.


# 5 полезных примеров кода на Python

![preview](./jjqoxswcr5qbvgi5bvbqds8r2dy.jpeg)

Python — один из самых популярных языков программирования, чрезвычайно полезный и в решении повседневных задач. В этой статье я вкратце расскажу о 22 полезных примерах кода, позволяющих воспользоваться мощью Python.

Некоторые из примеров вы могли уже видеть ранее, а другие будут новыми и интересными для вас. Все эти примеры легко запоминаются.

## 1 Получаем гласные

 Этот пример возвращает в строке найденные гласные *"a e i o u"*. Это может оказаться полезным при поиске или обнаружении гласных.

```python 
    def get_vowels(String):
    return [each for each in String if each in "aeiou"]
    get_vowels("animal") # [a, i, a]
    get_vowels("sky") # []
    get_vowels("football") # [o, o, a]
```

 ## 2  Первая буква в верхнем регистре

Этот пример используется для превращения каждой первой буквы символов строки в прописную букву. Он работает со строкой из одного или нескольких символов и будет полезен при анализе текста или записи данных в файл и т.п.

```python
    def capitalize(String):
    return String.title()
    capitalize("shop") # [Shop]
    capitalize("python programming") # [Python Programming]
    capitalize("how are you!") # [How Are You!]
```
## 3 Печать строки N раз

Этот пример может печатать любую строку n раз без использования циклов Python.

```python
    n=5
    string="Hello World "
    print(string * n)  #Hello World Hello World Hello World Hello World Hello World
```

## 4 Объединяем два словаря

Этот пример выполняет слияние двух словарей в один.

```python
    def merge(dic1,dic2):
        dic3=dic1.copy()
        dic3.update(dic2)
        return dic3
    dic1={1:"hello", 2:"world"}
    dic2={3:"Python", 4:"Programming"}
    merge(dic1,dic2) # {1: 'hello', 2: 'world', 3: 'Python', 4: 'Programming'}
```

## 5 Вычисляем время выполнения

Этот пример полезен, когда вам нужно знать, сколько времени требуется для выполнения программы или функции.

```python
    import time
    start_time= time.time()
    def fun():
        a=2
        b=3
        c=a+b
    end_time= time.time()
    fun()
    timetaken = end_time - start_time
    print("Your program takes: ", timetaken) # 0.0345
```

############# Python!

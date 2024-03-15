## Project Tasks

This project involves writing type-annotated Python functions and defining variables according to specific requirements. Each task is outlined below along with its corresponding description and example usage.

### Task 0: Basic annotations - add

Write a type-annotated function `add` that takes two `float` arguments `a` and `b` and returns their sum as a `float`.

Example:
```python
add = __import__('0-add').add

print(add(1.11, 2.22) == 1.11 + 2.22)
print(add.__annotations__)
```

### Task 1: Basic annotations - concat

Write a type-annotated function `concat` that takes two `str` arguments `str1` and `str2` and returns their concatenated string.

Example:
```python
concat = __import__('1-concat').concat

str1 = "egg"
str2 = "shell"

print(concat(str1, str2) == "{}{}".format(str1, str2))
print(concat.__annotations__)
```

### Task 2: Basic annotations - floor

Write a type-annotated function `floor` that takes a `float` argument `n` and returns its floor as an `int`.

Example:
```python
import math

floor = __import__('2-floor').floor

ans = floor(3.14)

print(ans == math.floor(3.14))
print(floor.__annotations__)
print("floor(3.14) returns {}, which is a {}".format(ans, type(ans)))
```

### Task 3: Basic annotations - to string

Write a type-annotated function `to_str` that takes a `float` argument `n` and returns its string representation.

Example:
```python
to_str = __import__('3-to_str').to_str

pi_str = to_str(3.14)
print(pi_str == str(3.14))
print(to_str.__annotations__)
print("to_str(3.14) returns {} which is a {}".format(pi_str, type(pi_str)))
```

### Task 4: Define variables

Define and annotate variables with the specified values:

- `a`: an `int` with a value of `1`
- `pi`: a `float` with a value of `3.14`
- `i_understand_annotations`: a `bool` with a value of `True`
- `school`: a `str` with a value of `"Holberton"`

Example:
```python
a = __import__('4-define_variables').a
pi = __import__('4-define_variables').pi
i_understand_annotations = __import__('4-define_variables').i_understand_annotations
school = __import__('4-define_variables').school

print("a is a {} with a value of {}".format(type(a), a))
print("pi is a {} with a value of {}".format(type(pi), pi))
print("i_understand_annotations is a {} with a value of {}".format(type(i_understand_annotations), i_understand_annotations))
print("school is a {} with a value of {}".format(type(school), school))
```

### Task 5: Complex types - list of floats

Write a type-annotated function `sum_list` that takes a list of `floats` as input and returns their sum as a `float`.

Example:
```python
sum_list = __import__('5-sum_list').sum_list

floats = [3.14, 1.11, 2.22]
floats_sum = sum_list(floats)
print(floats_sum == sum(floats))
print(sum_list.__annotations__)
print("sum_list(floats) returns {} which is a {}".format(floats_sum, type(floats_sum)))
```

### Task 6: Complex types - mixed list

Write a type-annotated function `sum_mixed_list` that takes a list of `integers` and `floats` and returns their sum as a `float`.

Example:
```python
sum_mixed_list = __import__('6-sum_mixed_list').sum_mixed_list

mixed = [5, 4, 3.14, 666, 0.99]
ans = sum_mixed_list(mixed)
print(ans == sum(mixed))
print("sum_mixed_list(mixed) returns {} which is a {}".format(ans, type(ans)))
```

### Task 7: Complex types - string and int/float to tuple

Write a type-annotated function `to_kv` that takes a `string` `k` and an `int` or `float` `v` as arguments and returns a tuple. The first element of the tuple is the string `k`. The second element is the square of the int/float `v` and should be annotated as a `float`.

Example:
```python
to_kv = __import__('7-to_kv').to_kv

print(to_kv.__annotations__)
print(to_kv("eggs", 3))
print(to_kv("school", 0.02))
```

### Task 8: Complex types - functions

Write a type-annotated function `make_multiplier` that takes a `float` `multiplier` as an argument and returns a function that multiplies a float by `multiplier`.

Example:
```python
make_multiplier = __import__('8-make_multiplier').make_multiplier
print(make_multiplier.__annotations__)
fun = make_multiplier(2.22)
print("{}".format(fun(2.22)))
```

### Task 9: Let's duck type an iterable object

Annotate the function `element_length(lst)` with appropriate types. It takes a list `lst` as a parameter and returns a list of tuples, where each tuple consists of an element from the input list and its length.

Example:
```python
element_length =  __import__('9-element_length').element_length
print(element_length.__annotations__)
```

## Repository Information

- **GitHub Repository**: [alx-backend-python](https://github.com/username/alx-backend-python)
- **Directory**: 0x00-python_variable_annotations

This README file provides an overview of the tasks and how to use the provided functions and variables with type annotations. Each task is followed by its example usage and expected output.

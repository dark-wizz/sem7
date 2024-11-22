# Exploring Python

---

- Creating python programs
- Statements
- Building blocks
- Testing functions
- Strings, Lists and tuples
- String functions
- Sets
- Dictionaries
- Combining dictionaries
- Making copies
- Zip list
- Loops
- Dynamic programming
- Persistent variables.

---

### Part A

- [ ] How will you write a print statement to print the string
      `C:\new_folder\test.txt`
- [ ] Show the output of following loop
  ```python
  for count in range(5):
  	print(count, end = " ")
  ```
- [ ] Find the equivalent Python representation for the following expression.
  ```python
  score = 3*scale if x>10 else 4*scale
  ```
- [ ] What is `2 * list1` if `list1 = [30, 1, 2, 1, 0]`

---

- [ ] how do you fix there in the following statement?
  ```php
  title = "Chapter " + 1 3.11
  ```
- [ ] find the result of the expression `a = 2 * 3 + 4 % 5 - 3 // 2 + 6`
  > [!info]- Ans
  > 15

### Part B

- [ ] Interpret the following block of code.
  ```python
  i = 1
  while True:
  	if i%3 == 0:
  		break
  	print(i)
  	i += 1
  ```
- [ ] Show the output of following block of code.
  ```python
  n = 5
  for i in range(n):
  	for j in range(i, n):
  		print("*", end = " ")
  	print()
  ```
- [ ] Develop a Python program to find the elements that are divided by 5 or 7 from a list and display in ascending order.
  > [!info]- Ans
  >
  > ```python
  > l = [10, 14, 28, 25, 20, 35, 3, 12, 49, 50]
  > l = [x for x in l if x % 5 == 0 or x % 7 == 0]
  > l.sort()
  > print(l)  # [10, 14, 20, 25, 28, 35, 49, 50]
  > ```
  
- [ ] Develop a Python program to replace all vowels by \* in a string.
> [!info]- Ans
> ```python
> s = input("enter: ")
> v = ["a", "e", "i", "o", "u", "A", "E", "I", "O", "U"]
> t = ""
> for i in s:
> if i in v:
> t += "*"
>     else:
>             t += i
>             print(t)
> ```

---

- [ ] show the return value of the following statements given `list1 = [30, 1, 2, 1, 0]` and `list2 = [1, 21 13]`
  - `list1 < list2`
  - `list1 <= list2`
  - `list1 == list2`
  - `list1 != list2`
  - `list1 > list2`
  - `list1 >= list2`
- [ ] translate the following expression into an equivalent python representation
  - `score = 3 * scale if x > 10 else 4 * scale`
  - `even = number % 2  == 0`
  - `y = 1 if x > 0 else -1`

### Part C

- [ ] Outline the operations of list datatype.
> [!note]- Notes
> ###### operation
> 1. indexing
> 2. slicing
> 3. concatination
> 4. updation
> 5. repetation
> 6. mambership
> 7. comparison
> ###### methods
> - a.append(e)
> - a.extend(arr)
> - a.push(e)
> - a.pop()
> - a.pop(e)
> - a.index(e)
> - a.sort()
> - a.reverse()
> - a.count()
> - a.pop()
> - len(a)
> - min(a)
> - max(a)
> - a.clear
- [ ] Summarize the methods of string datatype.
> [!note]- Notes
> ###### operations
> 1. indexing
> 2. concat
> 3. slice
> 4. repetation
> 5. membership
> 6. comaprison
> ###### methods
> - s.capitalize()
> - s.upper()
> - s.lower()
> - s.title()
> - s.swapcase()
> - s.split()
> - s.center(width, filller)
> - s.replace(old, new)
> - s.join(c)
> - s.isupper()
> - s.islower()
> - s.isalpha()
> - s.isdigit()
> - s.isalnum()
> - s.isspace()
> - s.title()
> - s.startswith(Str)
> - s.endswith(str)
> - s.find(substr)
> - len(S)
> - min(s)
> - max(s)

---

- [ ] illustrate the operations of list data type in python
- [ ] show the output of the following block of code

  ```python
  for i in range(1, 4):
    for j in range(1, 4):
      if i * j > 2:
        break
      print(i*j)
    print(i)

  ```

  ```python
  for i in range(1, 4):
    for j in range(1, 4):
      if i * j > 2:
        continue
      print(i*j)
    print(i)

  ```


# Introduction to PHP

---

- PHP
  - Introduction
  - Variables types
  - Understanding data types
  - Loose typing
  - Testing variable
  - Changing variables data type
  - Type casting
  - Operators and expressions
  - Operator types
  - Operator precedence Constants
  - Decisions and loops
  - Strings
  - Arrays
  - Functions.

---

### Part A

- [ ] Name the special data type in PHP
  > [!info]- Ans
  >
  > - NULL
  > - resouce
- [ ] Show the output of following operations if `x = 6` and `y = 3`.
  - x & y
  - x ^ y
    > [!info]- Ans
    >
    > - 2
    > - 5
- [ ] State the operation of <=>.
  > [!info]- Ans
  > spaceship operation
  >
  > - less - -1
  > - equal - 0
  > - more - 1

---

- [ ] State the output of
      ` $txt1 = "Hello"; $txt2 = "world"; echo $txt1 . $txt2`
  > [!info]- Ans
  > Helloworld
- [ ] List the categories of PHP data types.
  > [!info]- Ans
  >
  > - scalar
  > - compound
  > - special

### Part B

- [ ] Show a multidimensional array for the following table using PHP.

| Reg. No | Name | Grade |
| ------- | ---- | ----- |
| 1       | AAA  | S     |
| 2       | BBB  | A     |
| 3       | CCC  | B     |

- [ ] Demonstrate the use of array operations in PHP
  > [note]- Notes
  > +, ==, ===, !=, !==
- [ ] Interpret the following block of code
  ```php
  $s = 0;
  for($i = 1; $i <= 15; $i++){
  	if($i % 2 == 0){
  		continue;
  	}
  	$s += $i;
  }
  echo "Result: $s;"
  ```
- [ ] Outline a PHP script to check whether the given number is prime.

---

- [ ] illustrate break and continue statements in PHP
- [ ] demonstrate the use of variable length arguments

### Part C

- [ ] Explain looping statements in PHP with examples.
  > [!note]- Note
  >
  > - while
  > - do...while
  > - for
  > - foreach

---

- [ ] build PHP script to check whether a number
  - [ ] odd or even
	> [!note]- Note
    >
    > ```php
    > <?php
    > $v = readline("Enter a num: ");
    > if ($v%2==0) echo "even";
    > else echo "odd";
    > ?>
    > ```

  - [ ] prime or not
    > [!note]- Note
    >
    > ```php
    > <?php
    > $v = readline("enter a num: ");
    > $f = 0;
    > for($i=2; $i<=$v/2; $i++){
    >  if($v%$i==0){
    >    $f =1;
    >    break;
    >  }
    > }
    > if ($f) echo "not prime";
    > else echo "prime";
    > ?>
    > ```

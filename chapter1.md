---
title       : Chapter 1
description : R Basics. You will work with various data types (integers, numeric, characters) and learn how to assign variable.

--- type:NormalExercise xp:50 skills:1 key:1f9a0ebdf7
## Introduction

1. Introduction to RStudio [R studio 101] (http://dss.princeton.edu/training/RStudio101.pdf)
2. Intro to R Basics [Day 1 Lecture slides]
 
##### Learning how to use R Editor
1.*R Editor* - top right; *Console* - bottom right.
2. Type R code in the editor and hit the 'Submit Answer' button to execute R.
3. You will get a message whether or not your code was correct. 
4. The output of your R code is shown in the console.
5. Use console also to experiment cosing befre submiting.

##### Comments
R makes use of the `#` sign to add comments. The line with `#` at the beginning will not be executed. For example, _Calculate 3 + 4_ in the editor on the right is a comment. 


*** =instructions
- In the editor on the right you have some sample code. Which lines are actual R code and which are comments?
- Add a line of code that calculates the sum of 3 and 5
- Add a line with comment saying **This is my first script**
- Hit the 'Submit Answer' button.

*** =hint
Just add a line of R code that calculates the sum of 3 and 5.

*** =pre_exercise_code
```{r}
# no pec
```

*** =sample_code
```{r}
# Calculate 1 + 2
1 + 2

# Calculate 3 + 5




```

*** =solution
```{r}
# Calculate 1 + 2
1 + 2

# Calculate 3 + 5
3 + 5

# This is my first script
```

*** =sct
```{r}
test_output_contains("8", incorrect_msg = "Make sure to add `3 + 5` on a new line. Do not start the line with a `#`, otherwise your R code is not executed!")
success_msg("Awesome! See how the console shows the result of the R code you submitted? Now that you're familiar with the interface, let's get down to R business!")
```

--- type:NormalExercise xp:100 skills:1 key:b4b838e7e4
##Basic Data Types:
- Decimals values like `4.5` are called **numerics**.
- Natural numbers like `4` are called **integers**. Integers are also numerics.
- Boolean values (`TRUE` or `FALSE`) are called **logical**.
- Text (or string) values are called **characters**.

Assign a value with `<-`
`x <- 1`

Checking class `class(x)`

###Arithmetic Operators

- Addition: `+`
- Subtraction: `-`
- Multiplication: `*`
- Division: `/`
- Exponentiation: `^`


*** =instructions
- You have two numeric variables **x** and **y**
- Calculate their sum, substraction, multiplication, division, and exponentiation.
- Check class for **y**
- Click 'Submit Answer' and have a look at the R output in the console.

*Do not forget to scroll down your R editor*
*** =hint
Check class with `class()` function

*** =pre_exercise_code
```{r}
# no pec
```

*** =sample_code
```{r}
x <- 2
y <- 3
# An addition
x + y 

# A subtraction


# A multiplication


 # A division
 

# Exponentiation


# Check the class of y

```

*** =solution
```{r}
x <- 2
y <- 3
# An addition
x + y

# A subtraction
x - y 

# A multiplication
x * y

 # A division
x / y 

# Exponentiation
x ^ y

# Check the class of y
class(y)
```

*** =sct
```{r}
#msg = "Do not remove the other arithmetic examples!"
test_output_contains("x^y", incorrect_msg = "The exponentiation example is not correct. Write `x ^ y` on a new line.")
test_output_contains("x / y", incorrect_msg = "Write `x / y` on a new line.")
test_output_contains("x * y", incorrect_msg = "Write `x * y` on a new line.")
test_output_contains("x - y", incorrect_msg = "Write `x - y` on a new line.")
test_output_contains("class(y)", incorrect_msg = "Write `class(y)` on a new line.")
success_msg("Great! Head over to the next exercise.")
```

--- type:NormalExercise xp:100 skills:1 key:fcac6f7191
## Basic Data Types: Character

* A **character**  is used to represent string:
`name <- "John"`

* Character strings can be `paste` together:

 `fname <- Mary`
 
 `lname <- Johnson`
 
 `paste(fname,lname)`

* You can convert numeric into a character with `as.character(x)`

*** =instructions
- Create a variable with your first name (do not forget quotes)
- Create a variable with your last name (do not forget quotes)
- Paste two variables into one string
- Convert the number into a character string

*Do not forget to scroll down your R editor*
*** =hint
Remember characters must be enclosed into quotes, numbers are not.

*** =pre_exercise_code
```{r}
# no pec
```
*** =sample_code
```{r}
# Type your first name
fname <-

# Type your last name
lname <-

# Paste fname and lname


#Convert x into a character string
x <- 3


```
*** =solution
```{r}
# Type your first name
fname <- "[a-zA-Z]+"

# Type your last name
lname <-"[a-zA-Z]+"

# Paste fname and lname
paste(fname,lname)

#Convert x into a character string
x <- 3
as.character(x)
```

*** =sct
```{r}
test_output_contains("paste(fname,lname)", incorrect_msg = "Use paste function with two variables.")
test_output_contains("as.character(x)", incorrect_msg = "use as.character function - do not forget parenthesis.")
success_msg("Great! Head over to the next exercise.")
```

--- type:MultipleChoiceExercise xp:50 skills:1 key:5ba953ae37
## Data Type Quiz I

Select the correct data type for **x**

`x <- "3"` 
*** =instructions
- logical
- character
- numeric


*** =sct
```{r}
msg1 = "Try again! Think about quotes"
msg2 = "Well done. Proceed to the next exercise"
msg3 = "Try again! Think about quotes"
test_mc(correct = 2, feedback_msgs = c(msg1,msg2,msg3))
```

--- type:MultipleChoiceExercise xp:50 skills:1 key:a0f4522f4e
## Data Type Quiz II

Select the correct data type for **x**

`x <- TRUE` 
*** =instructions
- logical
- character
- numeric

*** =pre_exercise_code
```{r}
# no pec
```

*** =sct
```{r}

msg1 = "Well done. Proceed to the next exercise"
msg2 = "Try again!"
msg3 = "Try again!"
test_mc(correct = 1, feedback_msgs = c(msg1,msg2,msg3))
```

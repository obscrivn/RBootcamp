---
title       : Chapter 2
description : Vectors
  
--- type:NormalExercise xp:100 skills:1 key:960f76760f
## Creating Vectors

*** =instructions
- Create a vector with three characters a, b, c
- Create a vector with three numbers 1,2,3
*** =hint
Remember to use c() and characters must be with double quotes

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
myvector1 <- 

myvector2 <- 
```

*** =solution
```{r}
myvector1 <- c("a","b","c")

myvector2 <- c(1,2,3)
```

*** =sct
```{r}
test_object("myvector1", incorrect_msg = "remember these are characters")
test_object("myvector2", incorrect_msg = "remember these are numbers")
success_msg("Awesome!")
```
--- type:NormalExercise xp:100 skills:1 key:a251ab148d
## Working with Vectors
 
In this exercice you will practice:

* using ` length() ` 
* extracting elements from the vector

*** =instructions
- What is the length of the vector ` myvector1 `
- Find the 1st element of the vector ` myvector1 `
- Extract the first and the second elements
- Extract the 1st and the third elements
*** =hint
Remember to use length() and class()


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
myvector1 <- c("a","b","c")

# find the length of myvector1


# extract element 1


# extract element 1 and 2


# extract element 1 and 3
```

*** =solution
```{r}
myvector1 <- c("a","b","c")

# find the length of myvector1
length(myvector1)

# extract element 1
myvector1[1]

# extract elements 1 and 2
myvector1[1:2]

# extract elements 1 and 3
myvector1[c(1,3)]

```

*** =sct
```{r}
test_output_contains("length(myvector1)", incorrect_msg = "remember these are characters")
test_output_contains("myvector1[1]", incorrect_msg = "remember to use square brackets")
test_output_contains("myvector1[1:2]", incorrect_msg = "remember to use square brackets and slice")
test_output_contains("myvector1[c(1,3)]", incorrect_msg = "you need a vector of 1 and 3")
success_msg("Great!")
```
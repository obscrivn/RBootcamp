---
title       : Chapter 3
description : Lists

--- type:NormalExercise xp:100 skills:1 key:8156a925e3
## Creating List
List contains objects of different types. List is created with ` list() ` function.

*** =instructions
- Create a list that contains
* character **a**
* number **1**
* logical value **TRUE**
* a vector **c(1,2)**

*** =hint


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Create a list
my_list <- list()
```

*** =solution
```{r}
# Create a list
my_list <- list("a",1,TRUE,c(1,2))
```

*** =sct
```{r}
test_object("my_list", incorrect_msg = "make sure to use correct syntax")
success_msg("Awesome!")
```
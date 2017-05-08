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

--- type:NormalExercise xp:100 skills:1 key:ee74750bcd
## Indexing List
In this exercice you will practice slicing (finding) elements of the list
*** =instructions
- Find the length of the list
- Find the 1st element
- Find the 3rd element
- Extract the 1st element of the 3rd list element
* hint - you need to extract the word **my**


*** =hint
Remember to use double squre brackets and single square brackets

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# New list
my_list <- list("a",1,c("my","list"))

# Find the length of the list


# Find the 1st element


# Find the 3rd element


# Find the 1st element from the 3rd list element


```

*** =solution
```{r}
# Create a list
my_list <- list("a",1,c("my","list"))

# Find the length of the list
length(my_list)

# Find the 1st element
my_list[[1]]

# Find the 3rd element
my_list[[3]]

# Find the 1st element from the 3rd list element
my_list[[3]][1]

```

*** =sct
```{r}
test_output_contains("length(my_list)", incorrect_msg = "make sure to use correct syntax")
test_output_contains("my_list[[1]]", incorrect_msg = "make sure to use square brackets")
test_output_contains("my_list[[3]]", incorrect_msg = "make sure to use correct syntax")
test_output_contains("my_list[[3]][1]", incorrect_msg = "make sure to use correct syntax")
success_msg("Well done!")
```
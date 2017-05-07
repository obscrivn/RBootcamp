---
title       : Chapter 4
description : Setting up projects, directories and installing packages



--- type:NormalExercise xp:100 skills:1 key:4303b8ac87
## RStudio Review
[RStudio Screenshot] (https://iu.box.com/s/7631mxi7eyczxfu41l51hqzgi7fhubol)

Click on the link to view the screenshot

*** =instructions
- Examine the screenshot of RStudio
- In the R-Editor, complete the decsription of each of the four windowns in RStudio
- Choices are **console**, **packages**, **script**, **history** 
*** =hint


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
topleft <- ""

topright <- ""

bottomleft <- ""

bottomright <- ""
```

*** =solution
```{r}
topleft <- "script"

topright <- "history"

bottomleft <- "console"

bottomright <- "packages"
```

*** =sct
```{r}
test_object("topleft", incorrect_msg = "try again 1.")
test_object("topright", incorrect_msg = "make sure your string is spelled correctly.")
test_object("bottomleft", incorrect_msg = "try again 3.")
test_object("bottomright", incorrect_msg = "try again 4.")
success_msg("Awesome!")
```


--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:d729bc62a5
## Getting Help
You can consult ?help command if you need to learn about commands or functions.

Type in the console ` ?length `. Click `enter`. Can you tell what the command does?

Find now what the function ` aggregate `. Read the instructions and select the correct answer:


*** =instructions
- length of variable
- compute summary statistics
- concatenate string
*** =hint

*** =pre_exercise_code
```{r}

```
*** =sample_code
```{r}
#Type in the console 
?length

#Type in the console to find out about paste0

```
*** =sct
```{r}
msg1 = "Try again"
msg2 = "Well done!"
msg3 = "Try again"
test_mc(correct = 2, feedback_msgs = c(msg1,msg2,msg3))
```

---
title       : Starting with data
description : In this exercises, we'll import a dataset containing ecological data of animal species and weights. We'll then explore the data!
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf


--- type:NormalExercise lang:r xp:100 skills:1 key:e619cd064b
## Importing your data and first views

In this exercises, you'll import your ecological dataset. After doing so, you'll check out the first rows using the function `head()`. Make sure to read the information that this function call outputs to your console to get a first idea of ehat your data looks like. Happy importing!

*** =instructions
- Download the file from `"https://ndownloader.figshare.com/files/2292169"` to the location `"data/portal_data_joined.csv"`.
- Import the file from your local file system to a dataframe called `surveys`.
- Check out the first 5 rows of your data using the function `head()`.

*** =hint


*** =pre_exercise_code
```{r}
#Create dir for datasets:
dir.create("data")
```

*** =sample_code
```{r}
# Download the file to your local file system
download.file("https://ndownloader.figshare.com/files/2292169",
              "data/portal_data_joined.csv")

# Import the file into a dataframe: surveys              
surveys <- read.csv('data/portal_data_joined.csv')

# Check out your data!
head(surveys)

```

*** =solution
```{r}
# Download the file to your local file system
download.file("https://ndownloader.figshare.com/files/2292169",
              "data/portal_data_joined.csv")

# Import the file into a dataframe: surveys              
surveys <- read.csv('data/portal_data_joined.csv')

# Check out your data!
head(surveys)

```

*** =sct
```{r}


success_msg("Good work! Don't forget to look at the output of your work in the console and see what you can notice about the dataset that you have imported: what are the column names? What are the values?")
```



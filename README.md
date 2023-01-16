# WeRateDogs_TweetsAnalysis
The project is focused on implementing data wrangling skills and analysing the data to provide some insights for WeRateDogs tweeter account
## Project Objectives:
The main purpose of this project is to create a master dataset for WeRateDogs twitter account. The dataset will be used to bring some insights for them . Therefore, we will go through the following
process:
1. Gathering Data
2. Assessing Data
3. Cleaning Data
### Step 1: Gathering Data
In this phase, we have to gather the needed data in order to create our master dataset. There were 3 sources that had been found:
1. Direct Source from WeRateDogs account: receiving the twitter archive dataset through
email.
2. Finding a file on the internet: Downloading dogs breeds prediction file programmatically by
using a Request library, the prediction have been applied on WeRateDogs’ tweets.
3. Getting information from twitter API:
### Step 2 and 3: Assessing and Cleaning Data
After gathering and reading the collected file into Pandas dataframe, we have been assessed the 3
datasets to find any quality and tidiness issues.
#### Quality issues:
1.RatingDogs_df: there are 181 retweeted tweets, which they are a duplicated tweets not original tweet or from another users

2.RatingDogs_df: there's 23 records with rating_denominator that is larger or smaller than 10, some of them is a true rating and others doesn't has the right rating extraction

3.RatingDogs_df: name, dogge, floofer, pupper, puppo columns have none value as indicator of null

4.RatingDogs_df: most of the rows don't have a dog stage values, but i found out there's a number of values haven't extracted

5.RatingDogs_df: the name column has values that is not a name such as: a, an, the, and none as indicator of null

6.DogsBreeds_df: There's a 66 duplicated rows

7.DogsBreeds_df: There's a lot of predictions that are not a dog breed and 324 rows don't have any dog breed prediction

8.The datatype of ids and timestamp are not correct in all the datasets
#### Tidness issues:
1.RatingDogs_df: dogge, floofer, pupper, puppo columns are values not variable, so they should be in one column

2.DogsBreeds_df: There's multipule breed prediction with verious confidence for each dog

3.the 3 datasets need to be mereged since all of them about the same thing which is the dog.

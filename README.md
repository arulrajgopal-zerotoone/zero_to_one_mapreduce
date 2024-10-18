# zero_to_one_mapreduce
This repository provides a hands-on guide to MapReduce using the Python API.


#Pre-requiste
1. Ensure winget is installed already

            winget --version

2. install python 

            winget install Python.Python.3.9

2. Install mrjob

            pip install mrjob==0.6.12
   

# Execution through windows cmd prmpt
## Excercise-1
Calculate the average number of friends by age from the sample_data/fakefriends.csv file, which has the schema (ID, name, age, numFriends).

            python avg_friends_age.py sample_data/fakefriends.csv > outputfolder/avg_num_friends.csv



## Excercise-2
Find the frequency of each word from the give book file

            python word_frequency_counter.py sample_data/Book > outputfolder/words_frequency.txt


## Excercise-3
Input files: -

    u.item ->       user id | item id | rating | timestamp
    
    u.data ->       movie id | movie title | release date | video release date |
                    IMDb URL | unknown | Action | Adventure | Animation |
                    Children's | Comedy | Crime | Documentary | Drama | Fantasy |
                    Film-Noir | Horror | Musical | Mystery | Romance | Sci-Fi |
                    Thriller | War | Western | last 19 fields are genre, 1 indicates that genre

Find the most popular movie based on data file and lookup the item file to get movie name


            python most_popular_movie.py --items=sample_data/ml-100k/u.item sample_data/ml-100k/u.data > outputfolder/most_popular_movie.txt


## Excercise-4
Implement a recommendation system to find similar movies from the dataset used in Exercise 3.

            python movie_similarities.py --items=sample_data/ml-100k/u.item sample_data/ml-100k/u.data > outputfolder/sims.txt






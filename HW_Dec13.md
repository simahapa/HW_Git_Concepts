# HW_Git_Concepts
This is the HW for the  git concepts undertaken for the GA Data Science Course 

### Command Line Tasks
### 1.	Look at the head and the tail of chipotle.tsv in the data subdirectory of this repo. Think for a minute about how the data is structured. What do you think each column means? What do you think each row means? Tell me! (If you're unsure, look at more of the file contents.);
### Answer:
<br> Each column refers to the  following : </br>
<br> Order ID-unique ID of the order   </br>
<br> Quantity : refers to the how much of the item was ordered </br>
<br> Item_name: refers to what was ordered </br>
<br> Choice_description: Refers to the customization that  the order requested for by the customer </br>
<br> Item_price: refers to the price of the item </br>
<br>  </br>
<br>  </br>

### 2. How many orders do there appear to be?
<br>   </br>
### Answer:
*There are a  total of 1834 orders; the  command to perform the task is as follows
<br>   </br>
`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ tail chipotle.tsv
1831    1       Carnitas Bowl   [Fresh Tomato Salsa, [Fajita Vegetables, Rice, Black Beans, Cheese, Sour Cream, Lettuce]]       $9.25
1831    1       Chips   NULL    $2.15
1831    1       Bottled Water   NULL    $1.50
1832    1       Chicken Soft Tacos      [Fresh Tomato Salsa, [Rice, Cheese, Sour Cream]]        $8.75
1832    1       Chips and Guacamole     NULL    $4.45
1833    1       Steak Burrito   [Fresh Tomato Salsa, [Rice, Black Beans, Sour Cream, Cheese, Lettuce, Guacamole]]       $11.75
1833    1       Steak Burrito   [Fresh Tomato Salsa, [Rice, Sour Cream, Cheese, Lettuce, Guacamole]]    $11.75
1834    1       Chicken Salad Bowl      [Fresh Tomato Salsa, [Fajita Vegetables, Pinto Beans, Guacamole, Lettuce]]      $11.25
1834    1       Chicken Salad Bowl      [Fresh Tomato Salsa, [Fajita Vegetables, Lettuce]]      $8.75
1834    1       Chicken Salad Bowl      [Fresh Tomato Salsa, [Fajita Vegetables, Pinto Beans, Lettuce]] $8.75`

<br></br>

### 3. How many lines are in this file?
<br></br>
### Answer 

 <br> </br>

`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course`
<br></br>
`$ wc -l chipotle.tsv
'4623 chipotle.tsv`


### *The total number of lines in the data file is 4623 

<br></br>

### 4.	Which burrito is more popular, steak or chicken?


### Answer
Steak  has appeared a total of 706 times

`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ grep "Steak" chipotle.tsv|wc -l
706`
<br> </br>
<br> </br>
Chicken has appeared a total of 1565 times 
<br> </br>
<br> </br>
`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ grep "Chicken" chipotle.tsv|wc -l
1565`


### *On the basis of the above results where the chicken burrito appeared a total of 1565 times it is clearly more popular


<br></br>
### 5. Do chicken burritos more often have black beans or pinto beans?

### Answer 
<br> </br>
Total instances where chicken burrito was used 
`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ grep "Chicken Bu*" chipotle.tsv|wc -l
1279`


Total number of instances where Black beans were used is 282 
`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ grep "Black" chipotle_chickenb.tsv| wc -l
282`


Total number of times Pinto  Beans were used is 105 
`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
$ grep "Pinto" chipotle_chickenb.tsv| wc -l
105`


### *Hence, on the basis of the above findings the  chicken burritos have more black beans 

<br></br>

### 6. Make a list of all of the CSV or TSV files in the  (https://github.com/ga-students/DS-SEA-08). repo (using a single command). You will be working on your local repo on your laptop. Think about how wildcard characters can help you with this task.
<br></br>


### Answer 
Here is a list of all the csv and TSV files in the class repo
<br></br>
`$ find Documents/Siddharth/DS-SEA-08/data -name *.**v
Documents/Siddharth/DS-SEA-08/data/airlines.csv
Documents/Siddharth/DS-SEA-08/data/Airline_on_time_west_coast.csv
Documents/Siddharth/DS-SEA-08/data/bank-additional.csv
Documents/Siddharth/DS-SEA-08/data/bikeshare.csv
Documents/Siddharth/DS-SEA-08/data/chipotle.tsv
Documents/Siddharth/DS-SEA-08/data/citibike_feb2014.csv
Documents/Siddharth/DS-SEA-08/data/drinks.csv
Documents/Siddharth/DS-SEA-08/data/drones.csv
Documents/Siddharth/DS-SEA-08/data/hitters.csv
Documents/Siddharth/DS-SEA-08/data/icecream.csv
Documents/Siddharth/DS-SEA-08/data/imdb_1000.csv
Documents/Siddharth/DS-SEA-08/data/mtcars.csv
Documents/Siddharth/DS-SEA-08/data/NBA_players_2015.csv
Documents/Siddharth/DS-SEA-08/data/ozone.csv
Documents/Siddharth/DS-SEA-08/data/pronto_cycle_share/2015_station_data.csv
Documents/Siddharth/DS-SEA-08/data/pronto_cycle_share/2015_trip_data.csv
Documents/Siddharth/DS-SEA-08/data/pronto_cycle_share/2015_weather_data.csv
Documents/Siddharth/DS-SEA-08/data/rossmann.csv
Documents/Siddharth/DS-SEA-08/data/rt_critics.csv
Documents/Siddharth/DS-SEA-08/data/sms.tsv
Documents/Siddharth/DS-SEA-08/data/stores.csv
Documents/Siddharth/DS-SEA-08/data/syria.csv
Documents/Siddharth/DS-SEA-08/data/time_series_train.csv
Documents/Siddharth/DS-SEA-08/data/titanic.csv
Documents/Siddharth/DS-SEA-08/data/ufo.csv
Documents/Siddharth/DS-SEA-08/data/vehicles_test.csv
Documents/Siddharth/DS-SEA-08/data/vehicles_train.csv
Documents/Siddharth/DS-SEA-08/data/yelp.csv`

<br> </br>
*Here is another way to execute it:

`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS-SEA-08 (master)
$ find . -name *.*sv
./data/airlines.csv
./data/Airline_on_time_west_coast.csv
./data/bank-additional.csv
./data/bikeshare.csv
./data/chipotle.tsv
./data/citibike_feb2014.csv
./data/drinks.csv
./data/drones.csv
./data/hitters.csv
./data/icecream.csv
./data/imdb_1000.csv
./data/mtcars.csv
./data/NBA_players_2015.csv
./data/ozone.csv
./data/pronto_cycle_share/2015_station_data.csv
./data/pronto_cycle_share/2015_trip_data.csv
./data/pronto_cycle_share/2015_weather_data.csv
./data/rossmann.csv
./data/rt_critics.csv
./data/sms.tsv
./data/stores.csv
./data/syria.csv
./data/time_series_train.csv
./data/titanic.csv
./data/ufo.csv
./data/vehicles_test.csv
./data/vehicles_train.csv
./data/yelp.csv
./notebooks/GMapJson.csv`


<br></br>
### 7.	Count the approximate number of occurrences of the word "dictionary" (regardless of case) across all files of [our class repo] (https://github.com/ga-students/DS-SEA-8).

### Answer 
### *The approximate number of matches is #79 

`$ grep -r -i "dictionary" .|wc -l
79`

The ones in capital are also included below 

`./DS-SEA-08/code/00_file_reading.py:4. BONUS: Create a dictionary in which the key is the airline name (without the star)
./DS-SEA-08/code/05_api.py:# decode the JSON response body into a dictionary
./DS-SEA-08/code/05_api.py:# extracting the year from the dictionary
./DS-SEA-08/code/05_web_scraping.py:First, define a function that accepts an IMDb ID and returns a dictionary of
./DS-SEA-08/code/05_web_scraping.py:a list in which each element is a dictionary of movie information.
./DS-SEA-08/code/05_web_scraping.py:# define a function that accepts an IMDb ID and returns a dictionary of movie information
./DS-SEA-08/code/09_lambda_comprehension.py:# dictionary comprehension
./DS-SEA-08/code/99_pandas.py:    data dictionary: http://files.grouplens.org/datasets/movielens/ml-100k-README.txt
./DS-SEA-08/code/99_pandas.py:# create a DataFrame from a dictionary
./DS-SEA-08/data/rt_critics.csv:Janet Maslin,rotten,111418.0,New York Times,The film is so proud of its alleged daring that it even begins with a dictionary definition of the word 'deviant.' 'Sitcom' would have been more like it.,2003-05-20,14629.0,Threesome
./DS-SEA-08/data/sms.tsv:ham    There generally isn't one. It's an uncountable noun - u in the dictionary. pieces of research?
./DS-SEA-08/data/sms.tsv:ham    1) Go to write msg 2) Put on ` ### Dictionary### `mode 3)Cover the screen with hand, 4)Press  &lt;#&gt; . 5)Gently remove Ur hand.. Its interesting..:)
./DS-SEA-08/data/sms.tsv:ham    1) Go to write msg 2) Put on` ### Dictionary ### `mode 3)Cover the screen with hand, 4)Press  &lt;#&gt; . 5)Gently remove Ur hand.. Its interesting..:)
./DS-SEA-08/data/sms.tsv:ham    1) Go to write msg 2) Put on` ### Dictionary ### ` mode 3)Cover the screen with hand, 4)Press  &lt;#&gt; . 5)Gently remove Ur hand.. Its interesting..:)
./DS-SEA-08/data/yelp.csv:    Our photographer was wonderful. She seemed to enjoy her job and have fun with client's ideas. However the person who helped us pick out which cards to choose was not having any of it. If you looked up awkward in the dictionary and smacked them upside the head that's what it felt like. Her sheer agony of working there oozed out from her forced smile.
./DS-SEA-08/data/yelp.json:{"votes": {"funny": 1, "useful": 2, "cool": 1}, "user_id": "RwVaQNP1Ag-Seu3U9quGAg", "review_id": "6jV77Bs_Vu_rHkdUxu9JLQ", "stars": 3, "date": "2011-02-23", "text": "This review is for the JCPenny portrait studio responsible for the \"Christmas Blessings\" Christmas card that graced my family's and co-worker's mailboxes this past holiday season. \n\n    My girlfriend and I were going for a \"Step Brothers\" pose so we had to look the part. I guess the look won't be in any Vogue or GQ magazine this year. No, you'll have to go back to the time when Circus Magazine was popular and when mom and dad went to key parties. \n    \n    Our photographer was wonderful. She seemed to enjoy her job and have fun with client's ideas. However the person who helped us pick out which cards to choose was not having any of it. If you looked up awkward in the dictionary and smacked them upside the head that's what it felt like. Her sheer agony of working there oozed out from her forced smile. \n\n   Anyways, I'll just say that I am damn happy I had a coupon for a $30 package which included two 8x10s of different poses and a whompin' helping of greeting cards. A package that retails at about $170. \n\n   And no, even if you pay that price,  a happy ending is not included.", "type": "review", "business_id": "kwq3bK7BzPKLwXKqVRztHg"}
./DS-SEA-08/homework/00_python_practice_2.py:# dictionaries are made of key-value pairs (like a real dictionary)
./DS-SEA-08/homework/00_python_practice_2.py:# use the key to look up a value (fast operation regardless of dictionary size)
./DS-SEA-08/homework/00_python_practice_2.py:# accessing a list element within a dictionary
./DS-SEA-08/homework/03_python_homework_chipotle.py:PART 6: Create a dictionary in which the keys represent chip orders and
./DS-SEA-08/homework/04_command_line_chipotle.md:7. Count the approximate number of occurrences of the word "dictionary" (regardless of case) across all files of [our class repo] (https://github.com/ga-students/DS-SEA-8).
./DS-SEA-08/homework/06_yelp_votes_homework.ipynb:    "# each row is decoded into a dictionary named \"data\" using using json.loads()\n",
./DS-SEA-08/notebooks/.ipynb_checkpoints/03_correlation_exercise_ice_cream_and_car_data-checkpoint.ipynb:    "* [View the ice cream consumption data set data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/Ecdat/Icecream.html)"
./DS-SEA-08/notebooks/.ipynb_checkpoints/03_correlation_exercise_ice_cream_and_car_data-checkpoint.ipynb:    "* [View the Car Road Tests dataset data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/datasets/mtcars.html)"
./DS-SEA-08/notebooks/.ipynb_checkpoints/06_nba_knn-checkpoint.ipynb:    "- NBA player statistics from 2014-2015 (partial season): [data](../data/NBA_players_2015.csv), [data dictionary](../slides/06_nba_paper.pdf)\n",
./DS-SEA-08/notebooks/.ipynb_checkpoints/07_linear_regression-checkpoint.ipynb:    "We'll be working with a dataset from Capital Bikeshare that was used in a Kaggle competition ([data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data))."
./DS-SEA-08/notebooks/.ipynb_checkpoints/09_confusion_matrix-checkpoint.ipynb:    "- Data from Kaggle's Titanic competition: [data](../data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data)\n",
./DS-SEA-08/notebooks/.ipynb_checkpoints/09_titanic_logistic_regression_exercise-checkpoint.ipynb:    "- Data from Kaggle's Titanic competition: [data](../data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data)\n",
./DS-SEA-08/notebooks/.ipynb_checkpoints/10_bank_exercise-checkpoint.ipynb:    "- Data from the UCI Machine Learning Repository: [data](https://github.com/ga-students/ds-sea-05/blob/master/data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)\n",
./DS-SEA-08/notebooks/03_correlation_exercise_ice_cream_and_car_data.ipynb:    "* [View the ice cream consumption data set data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/Ecdat/Icecream.html)"
./DS-SEA-08/notebooks/03_correlation_exercise_ice_cream_and_car_data.ipynb:    "* [View the Car Road Tests dataset data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/datasets/mtcars.html)"
./DS-SEA-08/notebooks/06_nba_knn.ipynb:    "- NBA player statistics from 2014-2015 (partial season): [data](../data/NBA_players_2015.csv), [data dictionary](../slides/06_nba_paper.pdf)\n",
./DS-SEA-08/notebooks/07_linear_regression.ipynb:    "We'll be working with a dataset from Capital Bikeshare that was used in a Kaggle competition ([data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data))."
./DS-SEA-08/notebooks/09_confusion_matrix.ipynb:    "- Data from Kaggle's Titanic competition: [data](../data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data)\n",
./DS-SEA-08/notebooks/09_titanic_logistic_regression_exercise.ipynb:    "- Data from Kaggle's Titanic competition: [data](../data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data)\n",
./DS-SEA-08/notebooks/10_bank_exercise.ipynb:    "- Data from the UCI Machine Learning Repository: [data](https://github.com/ga-students/ds-sea-05/blob/master/data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)\n",
./DS-SEA-08/notebooks/11_advanced_sklearn.ipynb:    "- Wine dataset from the UCI Machine Learning Repository: [data](http://archive.ics.uci.edu/ml/machine-learning-databases/wine/wine.data), [data dictionary](http://archive.ics.uci.edu/ml/datasets/Wine)\n",
./DS-SEA-08/notebooks/13_natural_language_processing.ipynb:    "- **Notes:** Uses a dictionary-based approach (slower than stemming)"
./DS-SEA-08/notebooks/13_natural_language_processing.ipynb:    "    # create a dictionary of words and their TF-IDF scores\n",
./DS-SEA-08/notebooks/15_bikeshare_exercise.ipynb:    "- Capital Bikeshare dataset from Kaggle: [data](https://github.com/JamesByers/GA-SEA-DAT1/blob/master/data/vehicles_train.csv), [data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data)\n",
./DS-SEA-08/notebooks/16_ensembling.ipynb:    "- Major League Baseball player data from 1986-87: [data](../data/hitters.csv), [data dictionary](https://cran.r-project.org/web/packages/ISLR/ISLR.pdf) (page 7)\n",
./DS-SEA-08/other/python_reference:bool({})    # empty dictionary
./DS-SEA-08/other/python_reference:# create an empty dictionary (two ways)
./DS-SEA-08/other/python_reference:# create a dictionary (two ways)
./DS-SEA-08/other/python_reference:# convert a list of tuples into a dictionary
./DS-SEA-08/other/python_reference:# examine a dictionary
./DS-SEA-08/other/python_reference:# modify a dictionary (does not return the dictionary)
./DS-SEA-08/other/python_reference:# accessing a list element within a dictionary
./DS-SEA-08/other/python_reference:# string substitution using a dictionary
./DS-SEA-08/other/python_reference:# dictionary comprehension
./DS-SEA-08/project/README.md:* **Data dictionary (aka "code book"):** description of each variable, including units
./DS-SEA-08/README.md:* [Descriptions of Statistics terms in a straight forward way](http://stattrek.com/statistics/dictionary.aspx?definition=Probability_density_function) including density plot
./DS-SEA-08/README.md:* Exercise with NBA player data ([notebook](notebooks/06_nba_knn.ipynb), [data](/data/NBA_players_2015.csv), [data dictionary](/slides/06_nba_paper.pdf))
./DS-SEA-08/README.md:    * [Data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data)
./DS-SEA-08/README.md:* Exercise with Titanic data ([notebook](notebooks/09_titanic_logistic_regression_exercise.ipynb), [data](data/titanic.csv), [data dictionary](https://www.kaggle.com/c/titanic/data))
./DS-SEA-08/README.md:* Exercise with bank marketing data ([notebook](notebooks/10_bank_exercise.ipynb), [data](data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing))
./DS-SEA-08/README.md:* Review solutions to exercise with bank marketing data ([notebook](notebooks/solutions/10_bank_exercise_solutions.ipynb), [data](data/bank-additional.csv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing))
./DS-SEA-08/README.md:* Exercise with Capital Bikeshare data ([notebook](notebooks/15_bikeshare_exercise.ipynb), [data](data/bikeshare.csv), [data dictionary](https://www.kaggle.com/c/bike-sharing-demand/data))
./DS-SEA-08/README.md:    * [Data dictionary](https://cran.r-project.org/web/packages/ISLR/ISLR.pdf) (see page 7)
./DS-SEA-08/README.md:    * SMS messages: [data](data/sms.tsv), [data dictionary](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)
./DS_course/.ipynb_checkpoints/03_correlation_exercise_ice_cream_and_car_data-checkpoint.ipynb:    "* [View the ice cream consumption data set data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/Ecdat/Icecream.html)"
./DS_course/.ipynb_checkpoints/03_correlation_exercise_ice_cream_and_car_data-checkpoint.ipynb:    "* [View the Car Road Tests dataset data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/datasets/mtcars.html)"
./DS_course/00_python_practice_2.py:# dictionaries are made of key-value pairs (like a real dictionary)
./DS_course/00_python_practice_2.py:# use the key to look up a value (fast operation regardless of dictionary size)
./DS_course/00_python_practice_2.py:# accessing a list element within a dictionary
./DS_course/00_python_practice_21.py:# dictionaries are made of key-value pairs (like a real dictionary)
./DS_course/00_python_practice_21.py:# use the key to look up a value (fast operation regardless of dictionary size)
./DS_course/00_python_practice_21.py:# accessing a list element within a dictionary
./DS_course/00_python_practice_21SM.py:# dictionaries are made of key-value pairs (like a real dictionary)
./DS_course/00_python_practice_21SM.py:# use the key to look up a value (fast operation regardless of dictionary size)
./DS_course/00_python_practice_21SM.py:# accessing a list element within a dictionary
./DS_course/02_numpy_and_pandas-Copy1.ipynb:    "# this is a dictionary ; gives some keys and values \n",
./DS_course/03_correlation_exercise_ice_cream_and_car_data.ipynb:    "* [View the ice cream consumption data set data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/Ecdat/Icecream.html)"
./DS_course/03_correlation_exercise_ice_cream_and_car_data.ipynb:    "* [View the Car Road Tests dataset data dictionary](https://vincentarelbundock.github.io/Rdatasets/doc/datasets/mtcars.html)"
./DS_course/03_python_homework_chipotle.py.txt:PART 6: Create a dictionary in which the keys represent chip orders and
./DS_course/05_api.py:# decode the JSON response body into a dictionary
./DS_course/05_api.py:# extracting the year from the dictionary
./DS_course/05_api.py.txt:# decode the JSON response body into a dictionary
./DS_course/05_api.py.txt:# extracting the year from the dictionary`


### 8.	Optional: Use the the command line to discover something "interesting" about the Chipotle data. Try using the commands from the "advanced" section!


### Answer 

Total lines :

$ wc -l chipotle.tsv
4623 chipotle.tsv

;

Where as unique lines are as follows

`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS-SEA-08/data (master)
$ uniq -c chipotle.tsv >"test"
$ wc -l test
4589 test`

`User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS-SEA-08/data (master)
User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS-SEA-08/data (master)
$ wc -l chipotle.tsv
4623 chipotle.tsv`


### Ideally I would like to  find the  highest and the lowest spend for the list of orders and what the  mean, median and standard deviation is. I could not process the remainder of the topics 

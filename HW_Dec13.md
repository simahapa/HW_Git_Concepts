# HW_Git_Concepts
This is the HW for the  git concepts undertaken for the GA Data Science Course 
### Please refer to the file HW DS 2  to view the mark down file with the contents of the HW that is due on 12/13
### Command Line Tasks
1.	Look at the head and the tail of chipotle.tsv in the data subdirectory of this repo. Think for a minute about how the data is structured. What do you think each column means? What do you think each row means? Tell me! (If you're unsure, look at more of the file contents.);
### Answer:
<br> Each column refers to the  following : </br>
<br> Order ID-unique ID of the order   </br>
<br> Quantity : refers to the how much of the item was ordered </br>
<br> Item_name: refers to what was ordered </br>
<br> Choice_description: Refers to the customization that  the order requested for by the customer </br>
<br> Item_price: refers to the price of the item </br>
<br>  </br>
<br>  </br>
2. How many orders do there appear to be?
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

Make a list of all of the CSV or TSV files in the [our class repo] (https://github.com/ga-students/DS-SEA-08). repo (using a single command). You will be working on your local repo on your laptop. Think about how wildcard characters can help you with this task.
Here is a list of all the csv and TSV files in the class repo
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

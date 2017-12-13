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
There are a  total of 1834 orders; the  command to perform the task is as follows
<br>   </br>
'User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course
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
1834    1       Chicken Salad Bowl      [Fresh Tomato Salsa, [Fajita Vegetables, Pinto Beans, Lettuce]] $8.75'

<br></br>

3. How many lines are in this file?
<br></br>
The total number of lines in the data file is 4623 
 <br> </br>

'User@DESKTOP-CPCB3KP MINGW64 ~/Documents/Siddharth/DS_Course'
'$ wc -l chipotle.tsv'
'4623 chipotle.tsv'

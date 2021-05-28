# California Traffic Collision Data from SWITRS

<p align="center"> 
    <img src="https://i.ibb.co/wQQf9rG/tram-auto-crash-in-1957-frederiksplein-amsterdam.jpg" alt="SWITRS">
 </p>


This data comes from the California Highway Patrol and covers collisions from January 1st, 2001 until mid-October, 2020. [Alex Gude](https://alexgude.com/) has requested full database dumps from the CHP four times, once in 2016, 2017, 2018, and 2020. He has combined these datasets into the one presented here. For additional details, see Alex Gude's post: [Introducing the SWITRS SQLite Hosted Dataset](https://alexgude.com/blog/switrs-sqlite-hosted-dataset/)


There are three main tables:

* `collisions`: Contains information about the collision, where it happened, what vehicles were involved.
* `parties`: Contains information about the groups people involved in the collision including age, sex, and sobriety.
* `victims`: Contains information about the injuries of specific people involved in the collision.
There is also a table called case_ids which I used to build the other tables. It tells you which of the four original datasets each row came from.

There is a data dictionary [here](https://tims.berkeley.edu/help/SWITRS.php): He has in some cases remapped values so that they are human readable (making a left turn instead of D for example); you can find those mappings [here](https://github.com/agude/SWITRS-to-SQLite/blob/master/switrs_to_sqlite/value_maps.py).

<br>
<br>






**Goal of the homework**: Build a search engine over the "best books ever" list of [GoodReads](https://www.goodreads.com/). Unless differently specified, all the functions must be implemented from scratch. [Main Link](https://github.com/CriMenghini/ADM/tree/master/2020/Homework_3)


## Main Steps:
    > 1. Data conversion to MySQL
    > 2. Writing MySQL queries
    > 3. Data conversion to MongoDB
    > 4. Preprocessing using Python
    > 5. Writing MongoDB queries


## The repository consists of the following files:

1. __`ADM-HW3.ipynb`__: 
	> A Jupyter notebook which provides the solutions to all questions. The notebook consists of outputs, comments, theoretical answers and further explanations.
2. __`functions.py`__:
    > A Python script containing all the functions used in the `ADM-HW3.ipynb`.

# smallDAWG
Polystore implementation inspired by http://wp.sigmod.org/?p=1629

What
=========
Getting a consolidated view across data sources for better analytics. An example use case is looking at the movie lens data from the perpective of actual population distribution. This helps us understand if in some area (zip) we have more users/population ratio, which is a better populatrity indicator than just plain number of users.

Why
============
Seamless interface to disparate systems is tough. To understand the complexity refer [Michael Stonebraker's blog post](http://wp.sigmod.org/?p=1629). As the types of data and data sources have exploded, most interesting things can be pursued by the global view of the data. But as each data type and source works as an isolated island, getting this consolidated view is really tough. The original idea by  and subsequent work by [BigDAWG](http://users.eecs.northwestern.edu/~jennie/research/bigdawg_record.pdf) are great. If we focus just on data joins for analytics, we can relax some of the constraints mentioned in [BigDAWG guiding tenets](http://livinglab.mit.edu/wp-content/uploads/2016/01/bigdawg-polystore-system.pdf) and still accomplish a lot in a easier way with Spark and specifically Catalyst, this implementation is an attempt at that.

Who
===========
Anyone interested in data. "Data is the new oil" or any of the umpteen cliched lines and their target audience with a liberal dose of big/fast/I-have-no-clue data.

When
=======
The first use case with movie lens and US population will be up by 8th May 2016. Of course, this is a projection from me a person with a very high rate of failure and a proven track record of goofing up on all personal project work.

Results
============
Arrive at the user:population ratio for any zip code.


Developer Note
============
All experiments depend on data folder which is not checked in.
If you want to run them, create a folder called data and add the following data sets:
1. [movie lens data 10M](http://files.grouplens.org/datasets/movielens/ml-1m.zip)
2. [US population data](http://seer.cancer.gov/popdata/yr1990_2014.19ages/us.1990_2014.19ages.adjusted.txt.gz)

Tools is another folder which is not checked in, checkout
1. [wrangler](https://github.com/sans-sense/wrangler)
2. [openrefine](https://github.com/OpenRefine/OpenRefine)
3. [notebook](https://github.com/jupyter/notebook)




Tools
============

Why not mimic II
For all non-researchers like me getting to that data is tough, but the novelty of the data is in the different types of data that it already has. 

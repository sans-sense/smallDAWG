# smallDAWG
Polystore implementation inspired by http://wp.sigmod.org/?p=1629

What
=========
Getting a consolidated view across data sources for better analytics. An example use case is looking at the movie lens data from the perpective of actual population distribution. This helps us understand if in some area (zip) we have more users/population ratio, which is a better populatrity indicator than just plain number of users.

Why
============
As the types of data and data sources have exploded, most interesting things can be pursued by the global view of the data. But as each data type and source works as an isolated island, getting this consolidated view is really tough. The original idea by Michael Stonebraker in his [blog](http://wp.sigmod.org/?p=1629) and subsequent work by [BigDAWG](http://users.eecs.northwestern.edu/~jennie/research/bigdawg_record.pdf) are great. Some of these things can be easier with Spark and specifically Catalyst, this implementation is an attempt at that.

Who
===========
Anyone interested in data. "Data is the new oil" or any of the umpteen cliched lines and their target audience with a liberal dose of big/fast/I-have-no-clue data.

When
=======
The first use case with movie lens and US population will be up by 8th May 2016. Of course, this is a projection from me a person with a very high rate of failure and a proven track record of goofing up on all personal project work.

Results
============
Arrive at the user:population ratio for any zip code.


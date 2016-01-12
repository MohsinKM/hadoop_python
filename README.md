# hadoop_python
This project for udemy lecture; Taming Big Data with MapReduce and Hadoop

## Development
### Preparation
Use python(<=2.7.10) and MRJob library
* MRJob library install (perhaps, you need administrator privilege)
```console
> pip install mrjob
```

If you are using Windows, it is recommended to use Enthought Canopy in this lecture. (it looks like IDE for python; provide editor and consoles internally)

> URL: <https://www.enthought.com/products/canopy/>

### Data
Basically, all data have been placed respectively in '/data' directory before execution.

* [Movielens](http://grouplens.org/datasets/movielens/ "Movielens")

In this project, we use ml-100k

```console
> wget http://files.grouplens.org/datasets/movielens/ml-100k.zip
```

* Fake Friends data

> /data/fakefriends.csv

* Weather data from the year 1800

> /data/1800.csv

* Book data

> /data/book.txt


### Run
* Rating Counter with ml-100k data
```console
> python app/RatingCounter.py data/ml-100k/u.data
```

* Average Friends by Age with Fake Friends data
```console
> python app/FriendsByAge.py data/fakefriends.csv
> python app/FriendsByAge.py data/fakefriends.csv > dist/friendsbyage.txt
```

* Finding Temperature Extremes

Get minimum temperature by location
```console
> python app/MinTemperatures.py data/1800.csv > dist/mintemps.txt
```

Get maximum temperature by location
```console
> python app/MaxTemperatures.py data/1800.csv > dist/maxtemps.txt
```

* Word Frequency (However, it still make some errors)
```console
> python app/WordFrequency.py data/Book.txt > dist/wordcount.txt
```

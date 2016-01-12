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


### Run
* Rating Counter of ml-100k data
```console
> python app/RatingCounter.py data/ml-100k/u.data
```

* Average Friends by Age with Fake Friends data

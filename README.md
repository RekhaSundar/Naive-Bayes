# Naive-Bayes
Python 3

A program that implements a 2-class Naive Bayes algorithm with an apriori decision rule using a multinomial estimation for the classes and a gaussian estimation for the attributes. The formulas to be used are therefore:

<img width="596" alt="Formula1" src="https://user-images.githubusercontent.com/56769691/116668908-92b13e80-a9bb-11eb-8d0a-4ee6ad35ac22.png">

where xa is an instance x with an attribute a and μ and σ being the parameters of the Gaussian. The parameter estimates are given as follows:

<img width="305" alt="Formula2" src="https://user-images.githubusercontent.com/56769691/116669017-b1173a00-a9bb-11eb-84b0-bca41bcf37d8.png">

<img width="504" alt="Formula3" src="https://user-images.githubusercontent.com/56769691/116669458-36025380-a9bc-11eb-8ca3-88a3d349e83a.png">

where nci is the amount of instances for class ci. Given are the two data sets named Example and Gauss2 as csv files. The program reads both data sets and treats the first value of each line as the class (A or B). The output of is comma separated values per data set, which contains a row for each class:

<img width="221" alt="Output" src="https://user-images.githubusercontent.com/56769691/116669185-e6bc2300-a9bb-11eb-8212-567067a6f8d0.png">

The last (third) row contains the absolute number of misclassifications for the data. Machine learning libraries are not used, only numpy 1.12.1 is employed. The program accepts the following parameters:

1. data - The location of the data file (e.g. /media/data/Example.tsv)

The figures below shows the data for the Example set and its Naive Bayes solution.

![Figure](https://user-images.githubusercontent.com/56769691/116669552-5c27f380-a9bc-11eb-92c4-fdd5119515ae.png)


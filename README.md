# Unsupervised-Learning-Clustering

K Means:

https://www.naftaliharris.com/blog/visualizing-k-means-clustering/

https://shapeofdata.wordpress.com/2014/03/04/k-modes/

https://www.datanovia.com/en/lessons/assessing-clustering-tendency/#methods-for-assessing-clustering-tendency

https://stats.stackexchange.com/questions/332651/validating-cluster-tendency-using-hopkins-statistic

Dataset link: https://cdn.upgrad.com/UpGrad/temp/929fe498-1032-4ad6-997e-e3c8c33853ea/Online+Retail.csv

Hierarchical Clustering:

http://www.saedsayad.com/clustering_hierarchical.htm

https://stats.stackexchange.com/questions/195446/choosing-the-right-linkage-method-for-hierarchical-clustering

http://www.stat.cmu.edu/~ryantibs/datamining/lectures/05-clus2.pdf

K-Mode CLutering:

Dataset: https://ml-course3-upgrad.s3.amazonaws.com/Unsupervised+Learning_+Clustering/Other+Forms+of+Clustering/bankmarketing.csv

DBSCAN ALgo:

DB Scan Clustering
This is reading session, you are required to go through the text and understand the basic idea behind DBScan. You may also go through the link provided at the end, to better understand the topic.

DBSCAN is a density-based clustering algorithm that divides a data set into subgroups of high-density regions. DBSCAN groups together point that are close to each other based on a distance measurement (usually Euclidean distance) and a minimum number of points. It also marks as outliers the points that are in low-density regions.

DBScan Parameters
DBSCAN algorithm requires 2 parameters:

Epsom or EPS
MinPoints or MinSamples.
 
EPS
EPS is a distance parameter that defines the radius to search for nearby neighbours. We can imagine each data point having a circle with radius EPS drawn around it. 

The value of EPS taken to cluster the data has a significant impact on the results. If the value of EPS is considered too small, decidedly fewer data points will be considered in one cluster, and a large part of the data will not be clustered. The un-clustered data points will be considered as outliers because they don't satisfy the number of points to create a dense region. If the EPS value is chosen to be very high, no real clusters will be formed as all of them will merge in the same cluster. The eps should be chosen based on the distance of the dataset (we can use a k-distance graph to find it), but in general small eps values are preferable. 

Min Samples
Min Samples or Min Points are the number of minimum points to form a dense region or cluster. For example, if we set the min_samples as 5, we need at least 5 points to form a dense cluster. 

Minimum points can be selected from some dimensions (D) in the data set, as a general rule min points >=D+1. 

The DBSCAN algorithm is used to find associations and structures in the data that are usually hard to find manually.

https://www.naftaliharris.com/blog/visualizing-dbscan-clustering/

https://netflixtechblog.com/tracking-down-the-villains-outlier-detection-at-netflix-40360b31732

https://www.oreilly.com/ideas/clustering-geolocated-data-using-spark-and-dbscan

https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf




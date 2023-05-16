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


Gaussian Mixture Model


K-Means algorithm’s inner-loop iterates over two steps:

Assign each observation 
Xi to the closest cluster centroid 
μk Update each centroid to the mean of the points assigned to it.
So, for K-Means, every data point is assigned to any of the one clusters, this is known as Hard Clustering or Hard cluster assignment.

Hard Clustering: In hard clustering, the data points are assigned to any one cluster completely. That means for hard clustering there is no consideration of uncertainty in the assignment of a data points. 

The limitations with hard clustering are that we tend to clusters even those data points in one of the clusters, even if the data point doesn't follow the clustering trend completely. Forex, If we want to cluster the set of customers into two groups say "High-Value Customers" and "Low-Value Customers", we will end up clustering the average value customers to any one of the clusters.

So to overcome this issue, we have a concept of Soft Clustering.

Soft Clustering: In soft clustering, the assignment of the data point to a cluster is based on the probability or likelihood of that data point to existing in that cluster. If we take the above example of clustering the customers into two clusters, we will be able to identify those customers who didn't fall in any one.

For soft clustering, we have an algorithm called GMMs or Gaussian Mixture Models. GMM has two advantages over K-Means: 

GMM is a lot more flexible regarding cluster covariance.
GMM model accommodates mixed membership.
We strongly suggest you go through the algorithm as GMMs can be applied to applications like "Speech Recognition", "Image Clustering", "Financial Applications". 

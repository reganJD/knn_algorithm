# knn_algorithm
I developed a k nearest neighbors algorithm and then utilized functions in R to work with real patient data. 

Here is a chart of the K values and their respective accuracy that I tested to find more information about utilizing the algorithm. I found the results of the kvalues to be surprising. After reading more in the text I found that I should make the k value odd so there are no ties when the voting takes place. I repeated all the larger k numbers with similar odd numbers.  After noticing the peak at 50, I decided to go much higher, although computationally expensive, and aware that it is unreasonably high, I just wanted to see what would happen. Since the square root of our training data is around 25, which seems to be ubiquitously recommended as the desired k value, I believe it would be somewhere around that number. However, we see a peak in accuracy around 10. I decided to run again with k=13 to see what was happening around that area. I think that the k value, although peaking at 50, would be a mistake as large k values can lead to under-fitting but small k values can lead to over-fitting. We do find a valley right at the square root of the training data and perhaps that is the best since the accuracy is still relatively high but not peaked, indicating some other issues are occurring

![knn_plot.pdf](https://github.com/reganJD/knn_algorithm/files/12457311/knn_plot.pdf)

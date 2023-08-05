# Spark_KNN
## 4-ranks and 4-cores
The experiments are averaged on 3 repeats. They used 4 ranks and 4 cores. The first three are the version using sorting. The later three used priority queue reduction and no sorting.
![image](https://github.com/ChengjunXi/Spark_KNN/assets/93487110/ac7f8e98-dfbb-4df5-86b7-e890fb875baf)

The average of performance using sorting is 52956. The average of performance using priority queue reduction is 15403. The improvement is 3.438 times by avoiding sorting. The correctness is proved by unanimous accuracy 0.525.

## 1-rank and 1-core
The experiments are averaged on 3 repeats. They used 4 ranks and 4 cores. The first three are the version using sorting. The later three used priority queue reduction and no sorting.
![image](https://github.com/ChengjunXi/Spark_KNN/assets/93487110/a34a4a74-882b-4d04-b325-7bb27d9c6195)
![image](https://github.com/ChengjunXi/Spark_KNN/assets/93487110/60c43857-816b-45b6-b866-1799fbf239fc)

The average of performance using sorting is 66307. The average of performance using priority queue reduction is 25204. The correctness is proved by unanimous accuracy 0.525. The running time statistics is as below table.

## Statistics

| Configuration \ Algorithm	| Using priority queue reduction | Using sorting |
| ----- | ----- |
| 4 ranks and 4 cores	| 15403	| 52956 |
| 1 rank and 1 core	| 25204	| 66307 |

The improvement of Spark using sorting is 66307/52956=1.252. The total improvement of Spark avoiding sorting is 4.305.




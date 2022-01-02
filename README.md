# note_genetic_algo
假設自變數x共n個，使用遺傳算法進行特徵提取(降維)k個(其中n>k):   
1.隨機生成w個序列，每個序列有k個int，均為0/1，代表選取了哪些feature  
2.根據各序列的x建立模型並對測試集預測，求得fitness(ROC/MSE/ACC)   
3.根據Fitness，從高至底，取m個parents(或以fitness之加權機率抽取parents等方法)做crossover生成次代(次代有機率發生mutation)  
4.反覆循環，直至達到指定世代結束


Reference:  
https://gist.github.com/Vini2/bd22b36ddc69c5327097921f5118b709#file-simpledemoga-java  
https://blog.csdn.net/Mr_Lowbee/article/details/86566949  
https://blog.csdn.net/littlely_ll/article/details/72625312  
https://towardsdatascience.com/feature-selection-with-genetic-algorithms-7dd7e02dd237  
https://www.kaggle.com/tanmayunhale/genetic-algorithm-for-feature-selection  

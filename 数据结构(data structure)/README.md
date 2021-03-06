==**排序思想**==

1. 比较相邻的元素。如果第一个比第二个大，就交换他们两个。
2. 对每一对相邻元素做同样的工作，从开始第一对到结尾的最后一对。在这一点，最后的元素应该会是最大的数。
3. 针对所有的元素重复以上的步骤，除了最后一个。
4. 持续每次对越来越少的元素重复上面的步骤，直到没有任何一对数字需要比较。

**==插入排序运用时需要注意的==**

直接插入排序对于**最坏的情况**（严格递减/递增的数组），需要比较和移位的次数为n(n-1)/2；

对于**最好的情况**（严格递增/递减的数组），需要比较的次数是n-1，需要移位的次数是0。

==**插入排序算法分析**==

直接插入排序的时间复杂度是O(n^2^)，空间复杂度是O(1)，同时也是**稳定排序**。

> **稳定排序**：待排序的记录序列中可能存在两个或两个以上关键字相等的记录。排序前的序列中Ri领先于Rj（即i<j）.若在排序后的序列中Ri仍然领先于Rj，则称所用的方法是稳定的。
>
> 比如int数组[1,1,1,6,4]中a[0],a[1],a[2]的值相等，在排序时不改变其序列，则称所用的方法是稳定的。

**==代码实现==**

==**加工后执行的结果**==
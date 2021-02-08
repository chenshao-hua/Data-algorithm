一、堆

堆是一个完全二叉树，可以用数组来保存它。
堆的实现包括以下步骤：

（1）创建堆：对顶的元素是最大或者最小的；

（2）调整堆：自下向上，或者自上向下进行调整，调整方式，就是交换；

（3）插入一个元素：将新元素插入堆底，自下向上调整；

（4）删除堆顶：将堆底和堆顶元素调换，调整堆最后删除被移到堆底的元素；

简而言之，所有的一起操作的都是为了保证堆是完全二叉树，这样保存是使用内存最少的，并且
能实现快速排序和查找最新小值或者最大值。

二、堆的应用

（1）优先级队列：合并小文件、高性能定时器

（2）TopK问题：维护一个大小为K的小顶堆（任何节点都小于左右节点），如果新来的元素比它大，
就删除堆顶插入这个元素，小于这个元素不做处理。

（3）中位数问题：维护两个堆，一个大顶堆，一个小顶堆，可以是一半或者某个特定百分比。在插入
完成后调整比例。
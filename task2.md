# TASK2
```scala
    val list0 = List(1,2,3,4,9)
    //将lst0中每个元素乘以2后生成一个新的集合
    val list1 = list0.map(x=> x * 2)
    //将lst0中的偶数取出来生成一个新的集合
    val list2 = list0.filter(x => x%2 == 0)
    //将lst0排序生成一个新的集合
    val list3 = list0.sorted
    //将lst0反转
    val list4 = list3.reverse
    //4个元素一组，类型为Iterator[list[Int]]
    val iter = list0.grouped(4)
    //将Iterator转换成List
    val list5 = iter.toList
    //将多个List压扁成一个List
    val list6 = list5.flatten
    val lines = List("hello java","hello scala","hello scala","hello python")
    //按空格切分，再压平
    val words = lines.map(_.split(" "))
    val flatwords = words.flatten
    val res = lines.flatMap(_.split(" "))
    //并行计算求和
    val arr = Array(1,2,3,4,5,6,7,8,9,10)
    val res1 = arr.sum
    //和线程有关每个线程计算一部分
    val res1 = arr.par.sum
    //按照特定的顺序进行聚合
    val res2 = arr.reduce(_+_)
    val res3 = arr.par.reduce(_+_)
    val res4 = arr.par.reduce(_+_)
    val res5 = arr.reduceLeft(_+_)
    //聚合
    val list7 = List(List(1,2,3),List(3,4,5),List(6,7,8))
    val res5 = list7.flatten.reduce(_+_)-->
    val res6 = list7.aggregate(0)(_+_.sum,_+_)
    val l1 = List(5,6,4,7)
    val l2 = List(1,2,3,4)
    //求并集
    val list = l1 union l2
    //求交集
    val ints = l1 intersect l2
    //求差级
    println(res5)
```

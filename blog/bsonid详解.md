# mongo bsonid 详解

## bsonid的结构
bsonid是一个12字节的值，前4个字节是unix时间戳的秒数，接着是三字节的机器码，然后是2字节的PID，最后是3个字节的增量
```
BSONID: 0-1-2-3---4-5-6---7-8---9-10-11
        time     machine  pid     inc
```





## 参考
[MongoDB中ObjectId的误区，以及引起的一系列问题](https://blog.csdn.net/xiamizy/article/details/41521025)
[http://bsonspec.org/](http://bsonspec.org/)
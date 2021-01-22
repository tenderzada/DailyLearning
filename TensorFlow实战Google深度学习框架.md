### Chapter2 Tensorflow环境搭建

***

#### **Protocol Buffer**

Protocol Buffer是谷歌开源的一个处理结构化数据的工具。

>所谓序列化，是将结构化数据变成数据流的格式，简单的说就是变为一个字符串。将结构化数据序列化，并从序列化之后的数据流中还原出原来的结构化数据，统称为处理结构化数据。

除了Protocol Buffer，XML和JSON是两种比较常用的结构化数据处理工具。

使用Protocol Buffer需要先定义数据**格式**，还原一个序列化数据的时候需要用到这个格式。而XML和JSON不需要，所以XML和JSON比较简单，而Protocol Buffer序列化出来的数据比XML小3到10倍，解析速度快20到100倍。

**Tensorflow中的大部分数据都是通过Protocol Buffer来组织的。**

#### Bazel

Bazel是谷歌开源的自动化构建工具，类比与Makefile、Maven等。

### Chapter2 Tensorflow入门

***

#### 张量的概念

张量可以简单理解为多维数组，其中零阶张量表示为标量（scalar),一阶张量为向量（vector),但是张量在tensorflow中的实现不是使用数组的形式，它只是对运算结果的**引用**。


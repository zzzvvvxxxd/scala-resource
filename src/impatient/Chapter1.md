# 第一章

【第一题】：

![](https://raw.githubusercontent.com/zzzvvvxxxd/scala-resource/master/src/impatient/resources/Chaper1_1.png)

【第二题】：

```scala
scala> import scala.math
import scala.math

scala> math.sqrt(3)
res1: Double = 1.7320508075688772

scala> res0 * res0
res2: Double = 8.999999999999998

scala> 3 - res1
res3: Double = 1.2679491924311228
```

【第三题】：

val，重新赋值会报错

【第四题】：

```scala
scala> "crazy"*3
res4: String = crazycrazycrazy
```

文档见scala doc中StringOps的*方法

【第五题】:

```scala
def max(that: Int): Int
// Returns this if this > that or that otherwise.
```

`10 max 2`表示将2和10比较，如果10大于2则返回10，否则返回2。

【第六题】

```Scala
scala> val bigInt = 2 : BigInt
bigInt: BigInt = 2

scala> bigInt pow 1024
res6: scala.math.BigInt = 179769313486231590772930519078902473361797697894230657273430081157732675805500963132708477322407536021120113879871393357658789768814416622492847430639474124377767893424865485276302219601246094119453082952085005768838150682342462881473913110540827237163350510684586298239947245938479716304835356329624224137216
```

或者：

```Scala
BigInt(2).pow(1024) 
```

【第七题】

```Scala
scala> import scala.BigInt
import scala.BigInt

scala> import scala.util.Random
import scala.util.Random

scala> BigInt.probablePrime(100, Random)
res10: scala.math.BigInt = 1236728448233407321392932582659
```

【第八题】

```scala
scala.math.BigInt(scala.util.Random.nextInt).toString(36)  
```

【第九题】

```scala
scala> val str = "hello"
str: String = hello

scala> str.reverse(0)
res0: Char = o

scala> str.takeRight(1)
res1: String = o

scala> str.take(1)
res2: String = h

scala> str(0)
res3: Char = h
```

【第十题】

`take`从字符串开头取若干个字符

`drop`是从字符串开头丢弃若干个字符

`takeRight`和`dropRight`和前两者方向相反，从字符串尾开始操作

`substring`更适合获取字符串中间的字串，其他四个方法适合获取两端的子串。
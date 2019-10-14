# relu 激活函数的优缺点及改进方法

在文章[梯度消失和梯度爆炸](https://github.com/buki26/InterviewQuestions/blob/master/answers/%E6%A2%AF%E5%BA%A6%E6%B6%88%E5%A4%B1%E5%92%8C%E6%A2%AF%E5%BA%A6%E7%88%86%E7%82%B8.md)中，已经提到过 sigmoid 作为激活函数存在的问题，即用 sigmoid 做激活函数梯度是不可能超过 0.25 的，这样经过链式求导之后，很容易发生梯度消失。

relu 的出现可以解决 sigmoid 梯度消失的问题，relu 的图像及导数图像如图所示：
![](https://github.com/buki26/image/blob/master/relu%E5%87%BD%E6%95%B0%E5%8F%8A%E5%85%B6%E5%AF%BC%E6%95%B0.png?raw=true)

因此它的优点有：
1、大于 1 时导数恒为 1，即避免上述梯度消失的问题
2、求导容易，速度快

局限性：
由于小于 0 部分的导数恒为 0，会导致一些神经元无法激活

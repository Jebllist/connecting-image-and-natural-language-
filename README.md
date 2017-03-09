# connecting-image-and-natural-language-
Andrej Karpathy 论文中文翻译
# 1. 引言
## 1.1 回顾
> 我们可能希望机器最终可以和人类在所有智能领域竞争，但是从哪一个开始最好呢？决定这个很困难。很多人认为这是一个非常抽象的活动将是最好的，比如下棋。也有人认为，提供一个具有很好的、可以用钱买的感官器官的机器，然后，教他理解和讲英语。这个过程按照一个小孩正常教学进行。我不知道正确的答案是什么，但是我认为这两个方法都应该被尝试。———阿兰.图灵,计算机器与智能(1950)


按照图灵的远大的愿景，人工智能邻域一个梦想是让计算机能够看见、理解我们丰富的视觉世界，赋予他们使用自然语言和我们交流的能力。

人能容易完成很多涉及复杂视觉识别和场景理解，使用自然语言交流和在这两者间的联合翻译的任务。比如，对于人来说，迅速看一眼衣服图片就可以指出和描述这个视觉场景的大量细节。已图1.1为例，我们可以看着这幅图片，很快指出并且给出一些描述：“一只橘色斑点的猫”，“红色轮的滑板车”，“棕色硬木地板”或者简单说整个图片内容是“骑着滑板的猫”。

**挑战** 对于我们，这个能力是如此自然和不费力，很容易忘记这个任务对于计算机是多么难。在计算机中，这幅图片被表示成一个很大的数字数组，这些数字表示在任意位置的亮度。![image](http://note.youdao.com/favicon.ico)
```math
2^{2}
```

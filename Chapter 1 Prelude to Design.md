# Chapter 1 设计序章

## 1. V0.1

早在 2014 年，我们重建了 C4 的核心，完成后觉得如果用一个应用程序来展示所有的例子会很不错。

试过了一些设计方案后，我们意识到这些例子的内容简直不适合设计放在一个应用程序里展示。<sup><a name="to1" href="#1">1</a></sup>

所以我们放弃了这个想法。

## 2. V0.2

第二个想法是做一个试验性的动态的 C4 logo，将它包装在一个应用程序里，给它带来一些不错的交互性。在 2014 年晚些时候<sup><a name="to2" href="#2">2</a></sup>我们将重点放在了新的动态 logo<sup><a name="to3" href="#3">3</a></sup> 的设计上。这个 logo 长这样：

![一个等距 logo 的不同配色方案](http://www.c4ios.com/images/cosmos/1/01.png)

我们开始设计 logo，在大量的关于品牌、设计、意义等想法中来回摇摆。最后，我们想要尝试一个等距 logo，它的线条不断变化，创造出一种奇特的视觉扭曲和效果。

![动态 C4 logo 的最初概念](http://www.c4ios.com/images/cosmos/1/02.gif)

在 Illustrator 中设计一个 logo 是件苦差事。由于我们追求动态效果，而 Illustrator 并不能帮我们裁剪图片并生成动态图像。此外，主要的难点不是在构造这个 logo<sup><a name="to4" href="#4">4</a></sup> 上，而是在将概念通过动画动态地渲染诠释出来。Jake（[jakemakes.com](jakemakes.com)）会做几个对比文件，然后传到我这，我就能够说出类似「好啦，哪几条线该移动到哪儿、什么时候移动、以及它们的移动时长」这样的话。

![动画中不同状态的关键帧](http://www.c4ios.com/images/cosmos/1/03.png)

所以，我为 Jake 构建一个小应用程序，让他可以在 Xcode 中使用。从本质上讲，他能够看到他在 Illustrator 中创造出来的设计图，并且可以通过使用像下面这样简单的函数调用在等距网格中追踪这些设计：

```
ln(4,10,6,12)
ln(0,10,10,10)
ln(8,8,10,8)
ln(8,8,8,10)
```

简单地画出设计稿后，Jake 将它们发给我，这样我就能确切地知道哪些线条在不同版本的 logo 间移动。 　　 　　

这是我为他写的其中一个版本的[示例](https://gist.github.com/C4Framework/fba7ee39e49b5e992270)。
　
![在一个等距节点上的动画](http://www.c4ios.com/images/cosmos/1/04.gif)

![在另一个等距节点上的动画](http://www.c4ios.com/images/cosmos/1/05.gif)

我们最后决定放弃这个想法，有两个原因。首先，我们不喜欢品牌的概念。第二，它会花费我们很长的时间去控制动画的移动时间和位置，这会使得我们专注于次要的东西而不是产品。

## 3. V0.3

第三个想法是第一种想法的延续，我们要重建 C4 的 Swift 版本的例子，同时引入一个新品牌。我们选择了构建新的示例而不是将旧的例子重新翻新。除此之外，我们要在应用程序中构建一些更复杂的、可以为之写教程的组件。

![关于如何架构 C4 例子的应用程序的手稿](http://www.c4ios.com/images/cosmos/1/06.png)

这个重点是展示 C4 能做什么，同时构建一些不错的组件，使得大家能够想要学习如何使用 C4 构建一个应用。例如，我们专注于视图之间的过渡转场，以及菜单本身。

![V0.3 的视觉概念。左图和中图：例子的设计；右图：C4Twitter 订阅流的设计](http://www.c4ios.com/images/cosmos/1/07.gif)

我们还开始使用 C4 组件来完成一个 Twitter 订阅流的界面动画和交互。我们有一些相当棒的关于 `UITableViewCell` 元素标题栏上的滑动特性，使得载入订阅流非常容易。我们认为如果能创造出一些人们可以丢到他们项目中的「组件」，这将会是 C4 的一个不错的特性<sup><a name="to5" href="#5">5</a></sup>。

静坐思考后发现这个思路并不是一个正确的方向。这种体验更像是一种解决方案，而不是一个应用或是一种经验，我们像是在列举需求的功能主义者。

## 4. V0.4

最后，我有时间使用 Alejandro 和我一起从去年 12 月底到今年整个 1 月份完成的 C4 新版本。因为在那时，我想要产生一些关于写好教程和网站内容的新的想法。所以，我们开始注意在电影和实验界面中已经大量存在的动画痕迹很重的风格。

![新探索的早期灵感](http://www.c4ios.com/images/cosmos/1/08.png)

C4 是一个完美处理这些工作的引擎，因为它在动画控制方面有着非常的强大的特性，此外它也有着很好的内在交互：你可以为屏幕设计具有未来感的界面。

最终，Jake 想出了一个很棒的基于星座和穿越宇宙的概念的主意。我们开始收集技术和美学作品来激发灵感。

![一些我们四处抓取的丢在 Slack 中的有关星座星图技术美学的图片](http://www.c4ios.com/images/cosmos/1/09.png)

几个小时后，Jake 开始重新将这些灵感重组为第一个视觉概念，一个可以成为 COSMOS 的东西。

![早期关于 COSMOS 的几个组成部分](http://www.c4ios.com/images/cosmos/1/10.jpg)

![App 内使用的占星术图标](http://www.c4ios.com/images/cosmos/1/11.png)

## 5. 后文

COSMOS 有一个独特的菜单，用于让用户在不同的星座之间跳转。所有的内容都显示在一个复杂视差背景只上，并且运用了大量的精心设计好的动画。这个想法让接下来每一步操作足够简单和优雅。

![COSMOS 之后版本的基础动画](http://www.c4ios.com/images/cosmos/1/12.gif)

此外，这个应用程序满足了我们的大量预期想要的东西。主要有：

1. 展示了 C4 的动画和交互能力
2. 具有一些独特的元素：比如菜单、背景视差
3. 设计工作流程包括使用一些前沿的软件，如 PaintCode
4. 包含很多漂亮的润色效果，例如在屏幕底部的小栏目
5. 不会过于复杂：只有单一视图和一个弹窗
6. 尽管它很简单，但实际上构建了很多东西，并且它提供了大量的教程材料
7. 是可交付的，而不是单单只是一个例子

这整个过程大概花费了一年，但是其中我们将精力花在项目上。如果压缩所有我们花在设计和构建的时间，尴尬地说，可能只要三周就能完成...

哪些花在要不要粉碎之前努力的时间给了我们一个新的视角：我们需要抛弃某些想法。这是确保你走在正确的道路上非常重要的一环。

---

#### 脚注

<a name="1">1.</a> 我们希望建立一些更深入的教程，而不仅仅重新创建 C4 原 Objective-C 的版本所做的 215 例子。<a href="#to1">↩</a>

<a name="2">2.</a> 这是忙碌的一年，我们在整个夏天和秋天没有太多的时间投入到 C4 当中。<a href="#to2">↩</a>

<a name="3">3.</a> 这也是重塑 C4 的开端。<a href="#to3">↩</a>

<a name="4">4.</a> Jake 的 Illustrator 切图都很优秀。<a href="#to4">↩</a>

<a name="5">5.</a> 我们还保留着我们的雷达组件。<a href="#to5">↩</a>


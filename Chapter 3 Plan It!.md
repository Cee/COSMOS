# Chapter 3 开始计划！

从现在开始我们会编写代码，很多的代码。所以，我们需要制定一个能够让生活变得更轻松可靠的计划。这个计划很简单：为应用的每个主要组件建立一个只有单个视图的控制器或者对象。在接下来的五个章节中，我们将分别关注下列的每个组件：

* Infinite Scrollviews （无限滚动视图）
* Astrological Signs（星座符号）
* Parallax Background（视差背景）
* Menu（菜单）
* Info Panel（信息面板）

## 1. 无限滚动视图 

为了能够无限滚动，我们需要构建一个 UIScrollView 的子类，让它能够不断循环，而不是到头或尾的时候发生弹跳效果。我们会给滚动视图的更新方法添加一些逻辑，然后我们将会在一个简单的项目中测试这些逻辑。稍后，我们将用这个新的对象来建立视差背景。

![](http://www.c4ios.com/images/cosmos/3/01.png)

## 2. 星座符号

在我们的应用中，我们会使用并复用图标和星座的指示方向来表示每个重要的星座符号。

在这里，我们会使用单例（Singleton）来创建我们需要的形状和指示方向，而不是将它们硬编码进背景和菜单中。我们将会建立一些逻辑，能够让我们使用自然语言来获取我们需要的数据。这能够让应用中其余的代码部分更加具有可读性。

![](http://www.c4ios.com/images/cosmos/3/02.png)

## 3. 视差背景

宇宙是广袤无垠的，所以我们也要构建一个组件能为我们的应用创造许多深度。堆积 8 个视差图层、创建各种不同图像、随机化以及精巧微妙的动画会带给应用程序的导航一个非常不错的感觉。

![](http://www.c4ios.com/images/cosmos/3/03.png)

## 4. 菜单

应用的核心是一个放射状的圆形菜单，它有一系列内置的动画来展开和隐藏它的内容。我们会从构建出初始和最终的状态开始，然后建立在这两个状态之间切换的动画。之后，我们将修改长按手势，作为打开菜单选择其中一个选项的方法。

![](http://www.c4ios.com/images/cosmos/3/04.png)

## 5. 信息面板

最后，我们要添加一个小的信息面板，它会从菜单中弹出来并展示一些关于 C4 以及如何找到这个教程的信息。这个面板会实现的非常简单，但是它能为我们提供使用推进控制器、弹出窗口和引用外部链接的机会。

![](http://www.c4ios.com/images/cosmos/3/05.png)
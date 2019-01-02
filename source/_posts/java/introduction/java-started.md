---
title: Java 开发入门篇 - 起航
tags: 
 - Java入门
 - Java
categories: 编程
date: 2018-12-28 19:00:00
---

> 最怕的东西，最应该去突破。

## 初衷

之前在[博客园](http://www.cnblogs.com/mfrank/)已经陆续发了几十篇文章，但总体并没有一个很好的串联，在内容编排上也存在较多问题，因此特地将之前的文章做一个整理，一是将原有文章进行润色，让表达更加生动清晰，二是尽可能的将各个知识点连接成线，整理出自己的一套体系，并剔除其中的错误。

本系列文章不会鼓吹Java怎么怎么好，也不打算尝试怂恿那些在Java边缘徘徊的人来学习Java，只想根据自己的学习经验来给那些想要学习Java却不得其法的人提供一点自己的经验和看法。

## 编程的世界观

编程写代码其实跟玩游戏很像，你不断学习，不断提升，然后写代码来完成各种工作的过程就像打怪升级，赚钱买装备，最终打倒BOSS的过程。

每一款好的游戏都有一个较为统一完整的世界观，也会有一个统一的背景设定，你需要先接受和理解这个设定的背景，然后慢慢了解这个游戏的完整世界观，这样才能真正融入这个游戏。

比如说，《剑网3》的世界观设计一直遵循“纯武侠，真江湖”设计，背景设定便是唐宋时期，武林纷争，各大门派先后崛起，而你出身草芥，通过自身努力加入门派，然后通过不断修炼内功和挑战各种任务来提升自我。

又比如《饥荒》是关于一名科学家被恶魔传送到了异世界荒野的故事，游戏的主题是生存，所以你的目标是尽可能的利用各种资源来存活更长时间，同时要抵御各种外来威胁来保证自己的安全。

如果把编程开发也比作游戏的话，它更像是《我的世界》这样的自由度很高的沙盒游戏。有的人会将《我的世界》玩成一款生存游戏，享受被僵尸追杀的快感，有人会将它玩成一款建筑游戏，打造属于自己的王国。带着不同的目的人，会有完全不同的游戏体验。

编程也是如此，在编程的世界里，你拥有的是一个万能工厂，而你是一位工程师，在这里你可以生产出任何产品，汽车、轮船、火箭，如果你足够厉害，甚至可以创造一个新的世界，所有你需要做的，便是给出合格的设计图，接下来的事情，交给这个万能工厂就好了。

每个人拥有这个万能工厂的人都有着不同的目的，有的人只是为了参观，有的人是为了制作出性能强悍的跑车，有的人是为了制作自己用的小玩具。不同的目的就会有完全不同的体验，有的人会觉得枯燥，有的人会觉得无聊，而有的人会感觉激情四射。如果你能真正体会到其中的乐趣，那么你一定会爱上这个工厂。

但做出一张好的设计图并不是一件简单的事情，所以你需要不断的学习它的规范，设计出符合规范的设计图，才能被这个万能工厂正确生产出你想要的产品。等到你真正掌握了这个规范，就会发现，只满足于正确性还远远不够，于是渐渐的会开始追求效率和美感。为了提高设计效率，前辈们已经总结出很多种设计模式，适用于不同的设计场景，掌握了它们，在设计产品的时候便能更加随心所欲。

而关于编程美学，也是一门用经验堆积起来的学问。毕竟，作为工程师的我们，需要与其他工程师不断交流切磋，我们会观摩欣赏别人的设计图，也会把自己的设计图和别人探讨。所以设计图不仅仅是为了给这个万能工厂来运转，也是为了阅读。

当然，这都是后话了。

## Java编程的世界观

Java是一门高级编程语言，所谓的高级，是相对于汇编等机器语言而言的，有更高层次的抽象，更加接近自然语言和数学公式，基本脱离了机器的硬件系统。

前面说到，每种编程语言都是一个万能工厂，Java也有一个万能工厂。不同语言代表的不同工厂都有各自的擅长领域。目前来说，Java的主流应用领域便是Web/APP后端开发、嵌入式设备、大数据、安卓开发，当然，Java也可以开发桌面应用程序，也可以写游戏，但那些并不是Java擅长的领域。就像你可以用菜刀砍树，用斧头切菜一样，可以做，但是会有些别扭，有其他更好用的工具为什么要选择这样蹩脚的方式呢。不要忘了，这些工厂都只是一个工具而已，你的最终目的是实现你的要的功能。

简单来说，不管黑猫白猫，能抓住耗子的猫就是好猫。

所以对待各种编程语言，首先要保持理智，他们都只是一个工具，我们的目的是为了解决问题，不要陷入对某种语言的盲目崇拜的陷阱里，脱离场景而进行语言之间的对比是毫无意义的。

Java有很多开发方向，本系列文章将主要以JavaWeb开发为目标进行探索，利用Java这个大工厂来开发网站后端应用，为我们的前台页面提供强劲稳定的功能支持。

相对于桌面开发而言，JavaWeb开发更多的时候开发出的产品是默默的在后台工作的，需要通过前台html页面或者手机app，亦或是桌面app才能进行间接的交互。比如你打开淘宝，看到的那些页面架构和好看的图片大都是前端和UI的功劳，而你看到的那些文字内容，大都是后端的数据驱动的成果。（当然，现在可能更多的功劳又要归功于基于大数据的推荐系统了）

但不要因此而觉得Java后端开发很无聊，其实一个网站的后端就像一个程序的大脑，绝大部分的数据逻辑处理是由后端完成的，不仅要负责对数据进行处理，还需要跟数据库，各种消息中间件打交道，利用各种算法来实现特定的功能，比如根据销售数据进行热销推荐，对用户进行信用评级等等

前端则负责展示处理后的结果，并做出相应的响应，是一个应用的门面。前端侧重展示和交互，后端侧重程序的逻辑，都是为了提供更好的用户体验，只是着力点不一样而已。

Java这个大工厂能量无穷，想要完全掌控它的妙用需要一段较长的修炼时间，毕竟想要设计一张足够精巧的设计图纸并不是一件简单的事情，所以需要不断的学习。这个过程难免会遇到挫折和困难，其中很多坑对于新手而言是致命的，最简单的比如环境安装，很多人的兴趣就是夭折在环境的折腾上。其实很多坑，早有无数人踩过，也有很多人在网上分享过相关的解决办法，所以当你遇到问题的时候，可以先上百度找找，你要相信一定有人遇到过同样的问题，如果没找到，想想换个姿势搜索。

当然也许苦苦搜寻之后，还是无法解决你的问题，这时候，来自共同学习的小伙伴的支持就显得弥足珍贵了，为此，博主创建了一个QQ群【529253292】，这里也许可以找到你想要的答案。

Java的学习深造过程，就像是升级打怪过关卡，每个知识点都有些小boss，把它们打倒后便能获得相应的经验值，可以提升你的等级，但是随着你的等级的提升，这些小怪小boss对你的修炼的帮助已经聊胜于无了，于是你需要进行更艰难的修炼，去挑战更厉害的boss。

在这个世界里，自由度很大，大到也许会让刚接触的你迷失方向，不知所措。所以本系列文章将会提供给你一条前往JavaWeb开发的修炼道路，虽然并不一定是最优路线，但至少总体方向不会错，如果你刚好想往这个方向发展，那么本系列文章将会给你提供一些帮助。注意，本系列文章主张的是夯实基础，先修炼内功，然后再修炼外功，所以如果你想要的是捷径，想要知道如何在一两个月之内找到工作，那么这个系列文章可能不太适合你。

当你的经验累积到一定的值时，就能获得相应的头衔，在JavaWeb的发展中主要有两条升级路线，一条是技术路线，一条是管理路线，大致就像这样:

{% asset_img java-started-1.png JavaWeb升级之路 %}

两条路线的升级加点方式不太一样，但是都是当技术积累到一定程度后才能选择不同的升级路线。

所以，年轻的勇士，不要犹豫了，拿起你的桃木剑，在Java这个世界探索出自己的道路吧！
# 自学计算机科学

如果你是一个自学成才的工程师，或者从编程培训班毕业，那么你很有必要学习计算机科学。幸运的是，不必为此花上数年光阴和不菲费用去攻读一个学位：仅仅依靠自己，你就可以获得世界一流水平的教育💸。

互联网上，到处都有许多的学习资源，然而精华与糟粕并存。你所需要的的，不是一个诸如“200+免费在线课程”的清单，而是以下问题的答案：

*   你应当学习**哪些科目**，为什么？
*   对于这些科目，**最好的书籍或者视频课程**是什么？

在这份指引中，我们尝试对这些问题做出确定的回答。

## 简而言之

大致按照列出的顺序，借助我们所建议的教材或者视频课程（但是最好二者兼用），学习如下的九门科目。目标是先花100到200个小时学习完每一个科目，然后在你职业生涯中，不时温习其中的精髓🚀。

| 科目 | 为何要学？ | 最佳书籍 | 最佳视频 |
| --- | --- | --- | --- |
| **[编程](#编程)** | 不要做一个“永远没彻底搞懂”诸如递归等概念的程序员。| _《计算机程序的构造和解释》_ | Brian Harvey’s Berkeley CS 61A |
| **[计算机架构](#计算机架构)** | 如果你对于计算机如何工作没有具体的概念，那么你所做出的所有高级抽象都是空中楼阁。 | _《计算机组成与设计》_ | Berkeley CS 61C |
| **[算法与数据结构](#算法和数据结构)** | 如果你不懂得如何使用栈、队列、树、图等常见数据结构，遇到有难度的问题时，你将束手无策。| _《算法设计手册》_ | Steven Skiena’s lectures |
| **[数学知识](#数学知识)** | 计算机科学基本上是应用数学的一个“失控的”分支，因此学习数学将会给你带来竞争优势。| _《计算机科学中的数学》_ | Tom Leighton’s MIT 6.042J |
| **[操作系统](#操作系统)** | 你所写的代码，基本上都由操作系统来运行，因此你应当了解其运作的原理。 | _《操作系统导论》_ | Berkeley CS 162 |
| **[计算机网络](#计算机网络)** | 互联网已然势不可挡：理解工作原理才能解锁全部潜力。 | _《计算机网络：自顶向下方法》_ | Stanford CS 144 |
| **[数据库](#数据库)** | 对于多数重要程序，数据是其核心，然而很少人理解数据库系统的工作原理。 | _Readings in Database Systems （暂无中译本）_ | Joe Hellerstein’s Berkeley CS 186 |
| **[编程语言与编译器](#编程语言与编译器)** | 若你懂得编程语言和编译器如何工作，你就能写出更好的代码，更轻松地学习新的编程语言。| _《编译原理》_ | Alex Aiken’s course on Lagunita |
| **[分布式系统](#分布式系统)** | 如今，_多数_ 系统都是分布式的。 | _《分布式系统原理与范型》，第三版_  Maarten van Steen著 | 🤷‍ |

## 为什么要学习计算机科学？

软件工程师分为两种：一种充分理解了计算机科学，从而有能力应对充满挑战的创造性工作；另一种仅仅凭着对一些高级工具的熟悉而勉强应付。

这两种人都自称软件工程师，都能在职业生涯早期挣到差不多的工资。然而，随着时间流逝，第一种工程师不断成长，所做的事情将会越来越有意义且更为高薪，不论是有价值的商业工作、突破性的开源项目、技术上的领导力或者高质量的个人贡献。

> 全球短信系统每日收发约200亿条信息，而仅仅靠57名工程师，现在的 WhatsApp 每日收发420亿条。 
>
> — Benedict Evans (@BenedictEvans) [2016年2月2日](https://twitter.com/BenedictEvans/status/694342874729545729)

第一种工程师总是寻求深入学习计算机科学的方法，或是通过传统的方法学习，或是在职业生涯中永无止息地学习；第二种工程师
通常浮于表面，只学习某些特定的工具和技术，而不研究其底层的基本原理，仅仅在技术潮流的风向改变时学习新的技能。

如今，涌入计算机行业的人数激增，然而计算机专业的毕业生数量基本上未曾改变。第二种工程师的供过于求正在开始减少他们的工作机会，使他们无法涉足行业内更加有意义的工作。对你而言，不论正在努力成为第一种工程师，还是只想让自己的职业生涯更加安全，学习计算机科学是唯一可靠的途径。

> 23333 然而他们... [pic.twitter.com/XVNYlXAHar](https://t.co/XVNYlXAHar)
>
> — Jenna Bilotta (@jenna) [2017年3月4日](https://twitter.com/jenna/status/838161631662092289)


## 分科目指引

### 编程

大多数计算机专业本科教学以程序设计“导论”作为开始。这类课程的最佳版本不仅能满足初学者的需要，还适用于那些在初学编程阶段遗漏了某些有益的概念和程序设计模式的人。

对于这部分内容，我们的标准推荐是这部经典著作：《计算机程序的构造和解释》。在网络上，这本书既可供[免费阅读（英文版）](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html)，也作为[MIT的免费视频课程](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)。不过尽管这些视频课程很不错，我们对于视频课程的推荐实际上是[Brian Harvey 开设的 SICP 课程](https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter)（即 Berkeley 的 61A 课程）。比起MIT的课程，它更加完善，更适用于初学者。

我们建议至少学完SICP的前三章，并完成配套的习题。如果需要额外的练习，可以去解决一些小的程序设计问题，比如[exercism](http://exercism.io)。

如果你觉得SICP过于难，那我们推荐 _[How to Design Programs](http://www.htdp.org/)_ ；如果你觉得SICP过于简单，那我们推荐 _[Concepts, Techniques, and Models of Computer Programming](https://smile.amazon.com/Concepts-Techniques-Models-Computer-Programming/dp/0262220695/)_ 。

### 计算机架构

计算机架构——有时候又被称为“计算机系统”或者“计算机组成”——是了解软件底层的的重要视角。根据我们的经验，这是自学的软件工程师最容易忽视的领域。

_The Elements of Computing Systems_，又名“从与非门到俄罗斯方块”（“Nand2Tetris”），这本书规模宏大，让读者对计算机内的所有部分如何协同工作有完全的认识。这本书的每一章节对应如何构建计算机整体系统中的一小部分，
从用HDL（硬件描述语言）写基本的逻辑门电路出发，途经CPU和汇编，最终抵达诸如俄罗斯方块这般规模的应用程序。

我们推荐把此书的前六章读完，并完成对应的项目练习。这么做，你将更加深入地理解，计算机架构和运行其上的软件之间的关系。

这本书的前半部分（包括所有对应的项目）均可从[Nand2Tetris的网站上](http://www.nand2tetris.org)免费获得。同时，在Coursera上，这是一门[视频课程](https://www.coursera.org/learn/build-a-computer)。

为了追求简洁和紧凑，这本书牺牲了内容上的深度。尤其值得注意的是，流水线和存储层次结构是现代计算机架构中极其重要的两个概念，然而这本书对此几乎毫无涉及。

当你掌握了Nand2Tetris的内容后，我们接下来推荐Patterson和Hennessy二人所著的 _[《计算机组成与设计》](https://smile.amazon.com/Computer-Organization-Design-Fifth-Architecture/dp/0124077269)_，一本优秀的经典著作。这本书中的不同章节重要程度不一，因此我们建议根据Berkeley的[CS61C课程](http://inst.eecs.berkeley.edu/~cs61c/sp15/) “计算机架构中的伟大思想”来着重阅读一些章节。这门课的笔记和实验在网络上可以免费获得，并且在[互联网档案](https://archive.org/details/ucberkeley-webcast-PL-XXv-cvA_iCl2-D-FS5mk0jFF6cYSJs_)中有这门课程的过往资料。

[![Elements of Computing Systems](https://teachyourselfcs.com/elements-computing-systems.jpg)](http://www.nand2tetris.org) 

> 硬件是平台。
>
> — Mike Acton, Engine Director at Insomniac Games
([观看他在CppCon上的演说](https://www.youtube.com/watch?v=rX0ItVEVjHc))

### 算法与数据结构

正如几十年来的共识，我们认为，计算机科学教育所赋予人们的最大能量在于对常见算法和数据结构的熟悉。此外，这也可以训练一个人对于各种问题的解决能力，有助于其他领域的学习。

关于算法与数据结构，有成百上千的书可供使用，但是我们的最爱是Steven Skiena编写的 _[《算法设计手册》](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/)_。显而易见，他对此充满热爱，迫不及待地想要帮助其他人理解。在我们看来，这本书给人一种焕然一新的体验，完全不同于那些更加经常被推荐的书（比如Cormen，Leiserson，Rivest 和 Stein，或者 Sedgewick的书，后两者充斥着过多的证明，不适合以 _解决问题_ 为导向的学习）。

如果你更喜欢视频课程，[Skiena慷慨地提供了他的课程](https://www.youtube.com/watch?v=A2bFN3MyNDA&list=PLOtl7M3yp-DX32N0fVIyvn7ipWKNGmwpp)。此外，Tim Roughgarden的课程也很不错，
在Stanford的MOOC平台Lagunita，或者[Coursera](https://www.coursera.org/specializations/algorithms)上均可获得。Skiena和Roughgarden的这两门课程没有优劣之分，选择何者取决于个人品味。

至于练习，我们推荐学生在[Leetcode](https://leetcode.com)上解决问题。Leetcode上的问题往往有趣且带有良好的解法和讨论。此外，在竞争日益激烈的软件行业，这些问题可以帮助你评估自己应对技术面试中常见问题的能力。我们建议解决大约100道随机挑选的Leetcode问题，作为学习的一部分。

最后，我们强烈推荐 _[How to Solve It](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/)_。这本书极为优秀且独特，指导人们解决广义上的问题，因而一如其适用于数学，它适用于计算机科学。

[![算法设计手册](https://teachyourselfcs.com/skiena.jpg)](https://smile.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1848000693/) [![How to Solve It](https://teachyourselfcs.com/polya.jpg)](https://smile.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069116407X/) 

> 我可以广泛推荐的方法只有一个： 写之前先思考。
>
>— Richard Hamming

### 数学知识

### 操作系统

### 计算机网络

### 数据库

### 编程语言与编译器

### 分布式系统


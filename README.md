# tech-interview-handbook
## 说明
说明
这篇文章翻译自一位外国友人的关于面试的文章，我很喜欢这些文章。很系统的面试知识。刚好我在准备国外的面试，同时也需要准备英语就测试翻译了一下，希望对中文阅读者有一定的帮助。

由于本人第一次尝试翻译，所以可能存在不准确的地方。如果有读者发现有一些翻译有误或者不好的地方，请不吝赐教。

原文参见 [@Yangshun的: tech-interview-handbook](https://github.com/yangshun/tech-interview-handbook)


## 引言
### 关于软件工程师面试：你需要准备的一切
没有人有那么多时间去完成上千的LeetCode题目，好消息是你不必完成那么多题目也有机会从大厂拿到工作机会。

我在东南亚的共享汽车公司Grab的工作的并不开心，想进入FAANG，但我不知道如何去做。经过几个月的研究、学习和练习，我面试了11家公司，并成功拿到了湾区顶级科技公司的9份offer--Facebook、谷歌、Airbnb、Palantir、Dropbox、Lyft和一些初创公司。这是一个乏味的过程，我再也不想经历了。于是我写了这个指南，希望你不用再一步步查资料了。

本指南将—__快速概述关于如何准备软件工程师面试的最高技巧__--包括技术和非技术面试回合。在相关的地方，你可以通过访问本概述文章中的链接，或通过网站的左侧边栏，深入了解更多细节。

如何准备你的软件工程师面试：

1. 最大化你入选的机会
2. 搞清楚面试流程
3. 选择一门编程语言
4. 提高你的计算机基础
5. 练习编码面试
6. 准备系统设计面试（中高级工程师）
7. 准备行为面试
8. 薪资谈判

<h3>最大化你入选的机会</h3>

对于进入互联网大厂你觉得还有困难吗？第一个障碍可能是你的简历。

你的简历是进入互联网大厂的重要门票。在入围之后，你过去的成就与你的编码面试技巧相比明显变得不那么重要了。众所周知，编码面试技巧是可以有方法学习的。因此，能够很好地描述你过去的成就以通过筛选阶段是非常重要的。

不幸的是，即使是我个人认识的最有资格的候选人也不知道如何写好简历，而未能入围。事实上，当我们中的许多人没有入围的顶级科技公司时，我们往往认为我们的资格不足。但在大多数情况下，这可能只是缺乏良好的框架。

<h3>搞清楚面试流程</h3>
面试中可能会有很多阶段

1. 简单测试<br>
   频率：偶尔
   
   简单测试的目的是作为第一道筛选，以快速却有效的方式剔除极其薄弱的（甚至是非技术性的）候选人。它们是结构化的问题，有明确的答案，这使得它们可以由招聘人员/非技术人员或自动评分器来评判。这通常在招聘过程的前期进行。
2. 线上编码评估<br>
   频率：偶尔

   像简单测试一样，在线编码评估通常在面试的前期给出。给出的算法问题具有良好的输入和输出，考生要在在线编码界面上写代码来解决问题。HackerRank是一个非常常见的进行在线编码评估的平台。LeetCode将是在线编码评估中解决问题方面的一个很好的练习方式。然而，在HackerRank中，你通常要写代码从stdin中读取，同时打印到stdout，如果考生不熟悉API，就会被难住。
3. 带回家的任务<br>
   频率：罕见

   关于提出算法问题是否是评估个人能力的好方法，已经有很多争论，因为它们并不完全是工作中日常需要的最相关的技能。带回家的任务是一种旨在解决算法面试的缺点的形式，它让候选人在更大的项目上工作，使他们能够展示软件设计技能。

   然而，这种面试形式占用了候选人和公司的更多时间，因此在候选人数量众多的大公司中并不常见。这种形式在初创企业和小公司中更为常见。例子

   * 开发一上航班预订APP
   * 开发一个看板APP
   * 开发一个贪吃蛇小游戏

4. 电话或者视频面试<br>
   频率：常见

   电话面试是最常见的形式，每个候选人在面试时都会至少面对一次。你将被要求通过电话或VoIP（BlueJeans/Skype/Google Hangout）与面试官交谈。将给你一个问题，你将使用一个在线协作编辑器（CoderPad/CodePen/Google Docs）来处理这个问题。

   即使编辑器支持执行，通常也不允许你执行代码。所以不要依靠这个来验证你的解决方案的正确性。格式会因你申请的角色不同而略有不同。许多公司喜欢使用CoderPad进行协作式代码编辑。CoderPad支持程序的运行，所以有可能会要求你修正你的代码，使其可以运行。对于前端面试，许多公司喜欢使用CodePen，熟悉这种基于网络的编码环境的用户界面将是值得你花时间去了解的。

   
5. 线下面试<br>
   频率：必需

   如果你已经走到了这个阶段，恭喜你！这通常是决定录用前的最后阶段。进入现场面试阶段的候选人将被要求在办公室进行亲自面试。如果你是海外候选人，公司甚至可能让你飞过来并支付你的住宿费用。

   现场阶段通常包括多轮面试（编码、系统设计、行为），预计会持续几个小时。由于你是在现场，有可能你会被要求与面试官做白板练习，通常是解决一个算法问题或系统设计问题。也有可能你要带自己的笔记本电脑，在现场做一个项目/解决一个编码问题。

   对于小型（非上市）公司的现场面试，大多数会允许（而且更喜欢）你使用自己的笔记本电脑。因此，你提前准备好你的开发环境是很重要的。

   如果公司提供午餐，你也可能与员工共进午餐，在那里你可以了解更多关于公司文化。

<h3>选择一门编程语言</h3>

简历完成后，你的软件工程面试之旅的下一步很简单，不会花很长时间。决定一种编程语言。除非你面试的是移动或前端这样的专业职位，有特定领域的语言，否则你应该可以在算法编码面试中自由使用任何语言。

大多数时候，你心里已经有了一个--选一个你用得最多、最舒服的。编码面试中最常用的编程语言是Python、Java、C++和JavaScript。我不建议为了编码面试而学习一门全新的语言，因为要熟练掌握一门语言需要一段时间（平均至少需要几周），以便在面试时能够自如地挥洒自如，这本身就已经够紧张的了。我个人选择的编程语言是Python，因为它非常简洁，而且标准库提供的函数/数据结构。

<h3>学习和练习计划</h3>

下一步也是最重要的一步是练习解决你所选择的编程语言中的算法问题。虽然《Cracking the Coding Interview》是一个很好的资源，但我更喜欢通过实际解决问题来学习。

有很多平台可以用于此--如LeetCode、HackerRank和CodeForces。根据我的个人经验，LeetCode问题最适合用于面试准备，而HackerRank和CodeForces则更适合用于竞技编程。

然而，LeetCode有数以千计的问题，要知道从哪里开始，或如何组织你的实践，这可能是令人生畏的。我在这里提供了推荐的准备计划，也提供了结构化的资源。

<h4>学习计划</h4>

建议留出3个月的时间准备编码面试（每周11小时，即每天2-3小时），以便更全面的准备。我在这里分享了我的3个月学习计划，其中提供了一个编码面试主题清单，并附有资源和练习题，你应该每周按优先顺序进行练习。我也将很快增加推荐的1个月和1周学习计划的内容。

如果你有少于3个月的准备时间，你可以使用Grind 75工具（由我建立）生成你自己的学习计划，该工具根据你剩下的时间生成编码面试的推荐学习计划。其背后的算法包括按优先级对问题进行排名，也包括对所涉及的主题的广度和深度进行平衡。

<h4>可用的练习资源</h4>

在网络上，有很多资源在争夺你的注意力，很多资源只是在争夺你的钱，却没有提供任何价值。如果我必须确定优先次序--这些是我将串联使用的顶级编码面试准备资源。

1. [designgurus的算法课程](https://designgurus.org/course/grokking-the-coding-interview)
2. [AlgoMonster](https://shareasale.com/r.cfm?b=1873647&u=3114753&m=114505&urllink=&afftrack=)
3. 我的编码面试最佳练习指南（免费）
4. 我的编码面试技术指南（免费）
5. 我的算法学习指南（免费）
   
   [AlgoMonster](https://shareasale.com/r.cfm?b=1873647&u=3114753&m=114505&urllink=&afftrack=)
   
   除了通过练习和易懂的指南帮助你掌握重要的编码面试数据结构和算法问题外，AlgoMonster还有一个额外的好处，就是综合了常见的面试问题模式，你可以应用它来解决你以前从未遇到过的任何其他问题。由谷歌工程师制造，与LeetCode研磨的非结构化性质相比，这绝对是一个高质量的平台。数据结构和算法问题涵盖了所有常见的语言--Python、Java、C#、JavaScript、C++、Golang，以及更多。今天就加入，享受70%的折扣→。
   
   [designgurus的算法课程](https://designgurus.org/course/grokking-the-coding-interview)
   
   Design Gurus的这门课程扩展了推荐练习题的问题，但从问题模式的角度来进行练习，这也是我认同的学习方法，我本人也曾用这种方法在编码面试中获得了更好的成绩。该课程允许你用Java、Python、C++、JavaScript等语言练习选定的问题，还提供了这些语言的样本解决方案，以及一步步的可视化。学习和理解模式，而不是背诵答案! 今天就获得终身使用权 →
   
   我的编码面试最佳练习指南（免费）<br>
   如果你读过顶级科技公司使用的编码面试评估标准，你可能会对评估项目的数量以及如何持续展示雇用行为感到不知所措。
   
   这个编码面试最佳实践指南综合了编码面试前、面试中和面试后的可操作建议，以展示雇用信号。
   
   我建议在你练习编码面试问题时，将该指南内化并作为辅助工具，以确保你从一开始就培养良好的面试习惯和肌肉记忆。
   
   我的编码面试技术指南（免费）<br>
   有没有一种结构化的方法来增加你找到编码面试问题的好办法的机会？优化你的方法的时间和空间的复杂性如何？我的编码面试技巧指南教你一些处理你从未遇到过的问题的技巧--如问题可视化、用手解决、把问题分成子问题等。
   
   我的算法学习指南（免费）<br>
   我不确定这些是否有资格成为深度指南--它们更像是一页的 "学习小抄"，包括最好的学习资源、最好的LeetCode问题练习和需要记住的东西。然而，它们确保你涵盖所有最重要的理由，特别是在你没有时间的时候。因为这些也是帮助我争取到顶级技术offer的笔记--它们绝对有效。

<h4>尝试模拟面试</h4>

在面试官面前编码可能是一个令人紧张的经历，特别是如果你以前从未做过 - 这就是为什么获得实践经验是如此重要。

[interviewing.io](https://interviewing.io/)是目前市场上最好的模拟技术面试资源。它允许你与真正的谷歌和Facebook工程师预约模拟编码面试，尽管是匿名的。你甚至可以预订特定岗位的面试，如移动、前端、工程管理。甚至更好的是，如果你想更容易地过渡到现实世界的编码面试，你可以查看录制的面试，看看电话面试是什么样的。

此外，如果你在模拟面试中表现良好，你将能够解锁 "工作页面"，这使你能够直接预订Uber、Lyft、Quora、Asana等顶级公司的面试。我作为面试官和面试者都使用过[interviewing.io](https://interviewing.io/)，发现其体验非常好。

<h3>系统设计面试准备</h3>

如果你是一个中级或高级程序员，你可能期望系统设计问题成为你技术面试的一部分。LeetCode并没有充分涵盖这些问题，而且好的资源还很难得到。

系统设计面试的目的是评估候选人在设计涉及多个组件的真实世界软件系统方面的技能。

<h4>利用最好的系统设计面试准备资源</h4>
一些最好的系统设计面试准备资源包括:

1. [ByteByteGo](https://bytebytego.com/?fpr=techinterviewhandbook)--这是一个新的系统设计课程，由亚马逊上畅销的《系统设计访谈》书籍的作者Alex Xu编写。课程涵盖了系统设计的基础知识，然后深入探讨了10多个著名的普通产品（如设计YouTube、Facebook Newsfeed等）和多个大数据和存储系统（如设计一个聊天系统）的设计。对于每一次深入研究，都会对概念进行解释，并使用全面的图表，使其对任何资历的人都非常平易近人。
2. [grokking the System Design Interview by Design Gurus](https://designgurus.org/link/kJSIoU?url=https%3A%2F%2Fdesigngurus.org%2Fcourse%3Fcourseid%3Dgrokking-the-system-design-interview)--这可能是互联网上最著名的系统设计面试课程，它与其他大多数课程的不同之处在于它是纯文字的，这对于喜欢阅读而不是看视频的人来说是很好的（比如我自己！）。它包含一个流行的系统设计问题库，以及一个系统设计基础知识的词汇表。我个人已经完成了这个课程，并推荐许多人使用这个课程。强烈推荐!
3. [System Design Interview Course by Exponent](https://www.tryexponent.com/courses/system-design-interview?ref=techinterviewhandbook)--这门课程涵盖了系统设计的基础知识，并且有一个巨大的数据库，里面有流行的系统设计问题和模拟面试的视频。有些问题有文本答案，还有数据库模式和API供参考（我觉得这很有帮助）。虽然仅就系统设计面试内容而言，订阅费可能有点贵，但他们也提供了数据结构、算法和行为面试的高质量技术内容。一个涵盖技术面试准备所有方面的一站式平台，其便利性非常诱人。
4. ["Grokking the Advanced System Design Interview" by Design Gurus](https://designgurus.org/link/kJSIoU?url=https%3A%2F%2Fdesigngurus.org%2Fcourse%3Fcourseid%3Dgrokking-the-advanced-system-design-interview)--我还没有试过这个，但它是由创作《系统设计面试解惑》的人编写的，所以它应该是不错的 在我看来，你可能不需要这个，除非你是非常资深的人，或者要去找一个专家职位。

<h3>准备行为面试</h3>

每家顶级科技公司对软件工程师都至少有一轮行为面试。通常情况下，软件工程师的行为面试包括。分享简历上以前的经验细节 提供过去的情况和行为的例子，证明某些行为属性（如冲突管理，数据驱动） 分享野心和职业计划

尽管这些面试看起来很 "松散 "或没有结构，但实际上有一个结构化的方法来准备行为面试：

1. 使写STAR原则回答<br>
   STAR格式有助于你组织你对行为问题的回答。这最适用于要求你叙述过去的经历或行为的问题。情境。分享有关引起任务的情况的细节 任务。解释你需要实现的目标或你必须解决的问题，重点是你必须达到的范围、严重程度或具体基准或结果 行动。解释你做了什么来实现你的目标，描述你的选择和你如何做出决定 结果。描述你的行动的结果和你学到的东西
2. 练习程序员最常见的行为面试题<br>
   请参考软件工程师[最常见的30个行为问题](https://www.techinterviewhandbook.org/behavioral-interview-questions/)<br>
关于行为面试准备的更多提示，请参考我的[完整行为面试准备指南](https://www.techinterviewhandbook.org/behavioral-interview/)。

<h3>薪资谈判</h3>

最后，你在面试前绝对需要准备的最后一件事是软件工程师的薪酬谈判。在面试过程中的任何时候，关于工资的谈话都可能出现。我们也有关于谈判策略和软件工程师报酬的深入指南。

这就是我的全部内容--关于软件工程师面试准备过程中每一步的更多细节，请通过侧边栏或导航到下一页，深入了解我的手册中的每个主题。

## 取得面试
### 编写你的简历
## 编码面试准备
### 逐步分解如何准备编码面试
### 选择一门编程语言
### 学习和练习计划
### 实施：前中后
### 解决问题的技巧
### 模拟编码面试
### 编码面试的评判方法
## 系统设计面试准备
### 系统设计面试准备指南
## 行为面试准备
### 逐步分解如何准备行为面试
### 通用行为面试问题
### 准备自我介绍
### 准备你要问的问题
## 薪资相关谈判
### 理解薪资结构和福利
### 薪资谈判指南
### 谈判十大原则
### 公司之间的选择
## 算法学习备忘录
## 其它
### 公司面试流程
### 备注录
### 工程师等级
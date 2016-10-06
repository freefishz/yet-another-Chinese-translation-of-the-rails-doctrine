> 最近在 Ruby China 看到 @huacnlee 分享的 [The Rails Doctrine - 中文翻译](https://ruby-china.org/topics/30703)，拜读之下受益匪浅。
> 唯一遗憾是原译文不大符合我的阅读习惯，因此就有了这篇译文的诞生。希望与我有相似阅读习惯的小伙伴们会喜欢。:smile:
> 本翻译参考了 DHH 的原文 [The Rails Doctrine](http://rubyonrails.org/doctrine/) 和 @huacnlee 的译文，在这里对两位表示由衷的感谢！
> 译文中如有不当之处，欢迎指正。

# Rails 信条

Ruby on Rails 能够现象般地崛起并取得如此卓越的成就，很大程度上应归功于其对新技术的运用及切入的时机。但技术优势一般会随着时间推移而逐渐削弱，而好的时机也并不总会长久相伴。Rails 为何能始终保持与时俱进，并不断扩大其影响力和社区呢？这里有必要给大众一个合理的解释。我认为最主要的原因就是其一直坚守的那些饱受争议的信条。

这些信条在过去的十年中也在不断地演进，但最重要的依旧还是那些最基础的信条。我不会自诩是这些信条的原创者。毕竟，Rails 取得的最大的成就就是：围绕诸多离经叛道的思想（主要是关于程序设计和程序员本质），融合并培养了一个如此强大的社群。

闲话到此，以下就是 Rails 中最重要的9个信条，请用心领悟：

1. [尽可能地让程序员开心](#尽可能地让程序员开心)
2. [约定优于配置](#约定优于配置)
3. [主厨推荐](#主厨推荐)
4. [多元化](#多元化)
5. [推崇优美的代码](#推崇优美的代码)
6. [提供开发利器](#提供开发利器)
7. [面向综合应用](#面向综合应用)
8. [演进优于稳定](#演进优于稳定)
9. [兼收并蓄](#兼收并蓄)

## 尽可能地让程序员开心

没有 Ruby 就不会有 Rails，因此，第一信条必然是来自于创造 Ruby 的核心理念。

Ruby 最初的理念确实将 **程序员的开心** 放在最首要的位置，也就是将它放在许多曾经驱动程序设计语言和生态圈前进的真理之前。

当 Python 推崇 **完成一件事情，有且最好只有一种方式**，Ruby 却沉醉于表达方式的丰富多彩和优雅精妙。当Java因其保护程序员自身的特性而备受推崇，Ruby 却在欢迎工具里就附上了自尽的绳子。当 Smalltalk 专注于消息传递的纯粹性，Ruby 却近乎贪婪地增加关键字和构造器。

Ruby 如此与众不同是因为它非常尊重事物的多样性。而这些多样性中的绝大部分恰是为了满足程序员开心而服务的。这种追求不仅引起了 Ruby 与其他编程语言环境的争论，也开启了主流文化对 **究竟什么是程序员，以及他们应该如何工作的** 的认知。

Ruby 不仅了解程序员的编程感受，而且还会尽量满足甚至改善他们的编程感受。无论这些感受是不当的、异想天开的或是令人愉悦的。Matz 跨越了复杂度如此惊人的实现门槛，才让机器最终面带微笑以取悦它的人类伙伴。Ruby 充满了视觉假象，那些表面上看上去如此简洁、清晰和优美的代码，其背后的实现却如杂技般错综复杂。当然这些选择并不是没有代价的（不信的话，可以问问 JRuby 那些尝试对 Ruby 做逆向工程的人），这也恰恰是这些选择如此值得称赞的原因。

正是这种从另一个角度致敬程序设计和程序员的方式，使我深深的爱上了 Ruby。这不仅仅因为它的简单易用和充满美学的设计，也不是任何一项单一的技术成就，而是一种愿景，一种反文化。Ruby 就是程序设计领域中与现有专业程序设计模式相左，而又符合人类思维习惯的缺失部分。

我曾经说过，发现 Ruby 就像是找到了完全适合我大脑思维习惯的魔术手套。比我曾经梦想过的任何手套都要来得合用。它甚至成为了我从 **写程序只是因为我需要程序 ** 到 **写程序是因为我爱上了这种思维的运用和表达方式 ** 的转折点。就像是找到了 **流动之泉**（流动指的是著作 [Flow：The Psychology of Optimal Experince](http://www.amazon.com/Flow-Harper-Perennial-Modern-Classics-ebook/dp/B000W94FE6) 中描述的一种意识状态，处在这种状态中的人通常非常愉悦，富有创造力，并且完全沉醉其中），并能随意进入其中。熟悉 Csikszentmihalyi（上述著作的作者）著作的人都应该知道，这种影响力简直是有过之而无不及。

毫不夸张的说，Ruby 改变了我，并为我设定了人生努力的方向。这种启示是如此深刻，以致于让我对布道这个 Matz 的作品充满了使命感，也就是去传播这个意义深远的作品和它的优点。

读到这里，我可以想象你们中绝大部份的人都会难以置信地摇摇头。我不怪你们。当我对程序设计的认识还处在 **程序设计只不过是个工具** 的阶段时，如果有人跟我描述上述经历，我也会摇头的。并且，我还可能嘲笑这种过分夸张近似于宗教语言般的描述。但这确实是我的真实想法，也是我的肺腑之言，即便这也许会让某些人或绝大部分人感到不适。

无论如何，这对Rails来说究竟意味着什么，以及这个理念是如何指引 Rails 持续演进的呢？要回答这个问题，我想先来看看另一条早期经常被用来描述Ruby的原则是非常具有启发性的：最小惊奇原则。即 Ruby 应该如你预期般运行。通过以下与 Python 对比的例子可以非常容易地理解这个原则：

```rb
$ irb
irb(main):001:0> exit
$ irb
irb(main):001:0> quit


$ python
>>> exit
Use exit() or Ctrl-D (i.e. EOF) to exit
```

Ruby 可以同时接受 exit 和 quit 来退出终端交互界面，以此来满足程序员那显而易见的需求。而 Python 则会迂腐的指导程序员如何正确完成操作，即便它已经明确地知道程序员想要干什么（因为它给出了错误信息嘛）。这就是一个非常清晰而又短小的解释最小惊奇原则的例子。

最小惊奇原则最终在 Ruby 社区失宠的原因是：这条原则本身是非常主观的。最小惊奇原则，惊奇谁呢？显然是 Matz，以及那些和 Matz 具有相似思维方式的人。但是，随着Ruby社区的逐渐壮大，和Matz思维方式相左的人数比例也越来越多，这也成为了邮件列表里那些毫无意义的争论之源。因此，这条原则最终淡出了人们的视线，以避免 **甲男是否对乙物是否惊奇** 的争论无处不在。

但这跟 Rails 又有什么关系呢？其实，Rails 最初就是基于一个与最小惊奇（Matz）原则相似的原则设计的。这个原则就是DHH的 **璀璨微笑原则** ，简单来说就是：接口设计的最大考量是如何让我尽可能地开怀大笑。当我把这条原则写出来的时候，连我自己都觉得这听起来有些滑稽和自恋。

然而，正是由于这种最初的深度自恋才造就了 Ruby 或 Rails 这样的作品，并且这两个项目都是从单个作者的思想中迸发出来的。当然，这样说有将我自己的创作动机强加到 Matz 身上之嫌，因此我将声明缩小到我所知道的范围：我创作 Rails 纯粹是为了我自己。第一条也是最首要的原则就是为了能让我微笑。尽管 Rails 有各种各样的功能，但这些功能的最终目的都是为了能让我更好的享受人生，是为了帮助我改善为网络信息系统需求所争论不休的日常生活。

就像 Matz 一样，有时我也会做出一些愚蠢的决定来实现我自己的理念。其中的一个例子就是 Inflector，一个恰可以完成类到表映射的类（包含规则和不规则的情况），譬如 Person 类对应到 People 表、Analysis 对应到 Analyses，Comment 对应到 Comments。这种行为现在已成了 Rails 中毋庸置疑的一部分，但当我们还在宣扬该原则及其重要性的早期，争议的怒火曾经肆意蔓延。

另外一个例子是 **为了减少了些许实现的工作量，却几乎触发了大量程序员的恐慌** ，如：Array#second 到 #fifth（以及额外增加 #forty_two）。这些访问器别名曾严重冒犯了一位非常直言不讳的支持者，他认为这些过度设计（以及额外的那个 #forty_two 都接近文明的终点了。这是一个关于42的梗，请自行搜索答案，:smile: ）完全可以改写成 Array#[1]、Array#[2]（和 Array[41]）。

但是，时至今日上述两个决定依然能令我开怀。我非常享受可以在测试用例或终端里输入 people.third。这并不符合逻辑，也不高效，甚至有些病态。
但却能使我持续开怀，并由此充满信念并丰富我的人生，继而证明在服务了 Rails 12年之后依然参与其中是完全正确的选择。

和性能优化不一样，开心优化很难衡量。这使得开心优化几乎成了不科学的无谓之举。即使有些人并未完全放弃，但也觉得这是无关紧要的事情。因为程序员一直被教导要执着并攻克于可被衡量的事物，也就是那些可以明确指出A要比B好的事物。

尽管对开心的追求很难在微观角度加以衡量，但从宏观角度来看却很清晰。Ruby on Rails 社区中的很多人明显是因为这样追求的才聚集于此的。他们因拥有更好的，更能带来满足感的职业生涯而骄傲。而这条原则正好处于这些情感的汇集之地，可想而知它的成功是必然的。

因此，我们可以得出以下结论：尽可能让程序员开心可能是造就 Ruby on Rails 最关键的因素，它应该陪伴 Rails 一直走下去。


## 约定优于配置


## 主厨推荐


## 多元化


## 推崇优美的代码


## 提供开发利器


## 面向综合应用


## 演进优于稳定


## 兼收并蓄

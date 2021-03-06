# 4-2 商业模式：互联网如何赚钱


算法工程师的职业发展，是和算法工程师能为企业带来多大的价值正相关的。怎么样可以为公司带价值呢？**在商言商，公司的利润无非=收入-成本。**所以我们就从收入和成本两个方面来考量一下算法是否有什么发挥的空间。

**对于大多数互联网公司而言，边际成本通常比较低，所以如果能够把控住收入，基本上也就等于把控住了利润。**所以我们这篇文章就先重点分析一下收入的影响，然后再谈谈在成本控制上，算法可以发挥作用的地方。

为了讨论简单起见，下面的讨论我们都以To C的内容消费类的App为主：典型的代表就是抖音快手、今日头条、西瓜视频。

现在比较通用的说法是：内容消费的App的增长有三驾马车，分别是：UG(用户增长)、推荐、广告。严格的来说，广告的那个位置上，变现团队都应该算。因为现在变现的方式有广告、会员、直播等等，形式变化比较多。不过现在最流行的变现手段应该还是广告，为避免歧义，我们行文的逻辑先按照只有广告这一种变现方式来。

广告收入主要的途径是通过这个公式实现的：

**广告收入 = DAU × 用户平均使用时长 × 单位时长广告的曝光次数 × 广告点击率× 转化率 × 客单价 × 广告分成**

这个公式各个变量名称应该还比较好理解，就不具体解释每一个变量什么意思了。我们来研究一下这个公式，分开来看。

## DAU

首先最左侧的是用户规模DAU(Daily Active User，每日活跃用户)。DAU其实是一切产品收入规模的基础，类似的指标还有MAU(Monthly Active User，每月活跃用户)。所以大部分互联网向的App在公布自己的公司数据的时候，非常重要的一个指标就是自己的DAU/MAU数据，实在是因为DAU/MAU是一切收入的基础。

那么DAU具体是怎么形成的呢？我们具体来拆解一下。

**当前用户数 = f(用户新增，用户留存)**

当前用户的规模数，实际上是用户新增和用户留存的函数。当然还有其他的变量，比如回流用户数，就是一个用户来了，可能因为某些原因，这个用户流失了，过段时间他又来了。这种用户显然有别于一般意义上的新用户，通常被叫做回流用户。统计上一般把新用户的增长叫做”拉新”，回流用户再来叫做“拉活”，两者的策略某种程度上可以相同对待。

此外，影响当前用户规模数的还有App自身性质，比如打开的频率，比如抖音可能是天天打开，但工具类的App比如支付宝，是只有在使用的时候才会打开，这也会影响某一个时间点用户的DAU。

不过为了简单起见，在分析DAU时，我们还是分成用户**新增用户**和**用户留存**两个变量来分别进行拆解。

### 新增用户

用户的新增量受到哪些因素决定呢，其中比较重要的一个因素就是对外的广告和推广。

怎么样给自己的产品做广告其实背后是有学问的。常见的App广告的宣传方式一般有素材广告、品牌广告、预装等等。

我们首先来看一下素材广告。素材广告一般是指在其他App指定的广告位投放的广告。广告的内容可以是图文、视频、或者一个片段节选，这些被统称为素材。要制作一个好的素材广告，首先得知道在其他App的广告位是什么样的。比如抖音的广告位是竖屏的视频形式，而在豆瓣的广告位肯定就是图文类型。然后我们需要确定的素材本身，可以是一个代表性的内容(快来西瓜视频看虞书欣/孙燕姿的Vlog)、或者是请广告公司制作的片段。那应该选择什么样的素材呢？所以问题就转化成了，在众多可以选择的候选内容之中，选择哪些内容可以带来最多新用户？这就是一个比较明确的目标了，是一个可以建模或者进行统计分析的点。

接下来是品牌广告。品牌广告一般是指那些为了追求品牌的曝光而打的广告，一般会出现在一些公共场所，比如在楼梯间，公交站；或者是App的开屏、电视台的广告、综艺的冠名等等。选择在什么地方打广告，什么时候，打多久，这直接会决定受众是否看到这个广告，进而会决定因为这个广告产生的新增用户是否符合预期。品牌广告一个比较大的问题是不太好做归因：比如你在楼梯间看到了某一个品牌的广告，可能过了一会儿才想到了这个App决定下载尝试一下，这样新增用户就不再是因为品牌广告产生的了。所以品牌广告的统计分析更依赖一些经验。

还有一种用户增长的常见手段是预装。具体是指：用户购买到一个新的手机后，通常会发现在刚刚打开手机的时候就已经存在许多App。这意味着一个用户只要买了手机，就有可能成为这个App的潜在用户。这也是拉新用户的一个常见手段。这个手段在国内智能手机还没有完全普及的时候，伴随着大量的手机出货，可以用低廉的价格带来大量的新增。

这些渠道，或者说是方法：无论是素材的制作，品牌广告的投放，或者是手机预装，本身都是有成本的。而通过对外的广告带来的新增用户，如果最终在App内留存下来了，那从长期来看，这个用户大概率是可以为公司创造收入的(比如广告收入)，这个用户在长期在公司创造的价值，叫做LTV(Long Term Value)。这里面是有一套近似的估算方法，有点类似于保险精算的成本计算。

为了评估新增用户从收入成本的角度来说是否符合预期，人们定义了一个指标，叫做ROI。具体的计算方法是

**ROI = 用户长期能创造的收入(LTV) / 用户新增的成本**

我们就可以根据ROI的高低来衡量拉新的是否符合预期。

### 用户留存

接下来是用户留存。一般而言，用户留存受以下这几个因素的影响。

* 产品的基础体验：UI是否好看，产品逻辑是否符合逻辑，播放视频时候是否卡顿等等
* 内容推荐算法：推荐的商品和内容用户是否喜欢；是否有喜欢的作者；搜索的结果是否符合预期等等
* 产品自身的品牌

我们分开来说。用户来到一个产品。第一眼看到的是这个产品的UI，会尝试使用一两个基础的功能，这些功能基础体验上的好坏，会直接决定用户是否还会继续留在这个App(试想一下一个杂乱无章的UI上配着一个非常卡顿的页面，换谁都受不了)。产品的硬性指标，换句话说应该是用户的基础体验。所以我们需要UI、设计、客户端、服务端同学一起合作，给用户提供一个好的基础体验。

接下来用户会开始正式开始使用你这个App，会审视你这个App给他返回的内容是不是喜欢。这其实就是推荐算法开始发挥作用的地方了。所以我们需要一个好的推荐策略去承接新用户；还要保证，对于那些已经在App上有动作的用户，他的兴趣可以迅速收敛，让这个用户可以一直使用App，一直愉悦，停不下来，自然就留存了；对于那些已经使用了很久的老用户，我们要保证推荐的内容可以足够精准，帮助他筛选到自己想要的信息，保证他在这个App有足够的消费时长，同时可以留下来。

这时候用户可能会开始搜寻，这里是否有一些她自己之前听过名字的一些作者；同时可能会发现一些站内的特色——站内有一些其他平台没有的作者。从某种角度上来说，这些作者在站内首先得有，其次还能够分发出来。首先，保证作者在站内得有，对于有众多粉丝的大作者而言，需要作者运营同学的努力，通过某些手段和作者建立联系，个性化的满足这些作者的需求，同时帮助这些作者更好的在站内的环境下取得好的播放量和用户反馈。此外，运营的覆盖肯定不能覆盖所有的作者，推荐算法要能保证所有生产优质内容的作者可以推出来可以被用户看到，得到用户的反馈，同时，还得为小作者成长为大作者提供一个好的上升渠道。这一切都必须要得益于一个好的推荐算法分发的机制。

App品牌自身对用户的留存也很有影响。比方说，如果这时候市面上出现一个和抖音一模一样的App，就是不管从UI、内容、算法都一模一样，你是否还继续使用？大概率是不会的。因为你会觉得这个App太像抖音了，而你有抖音就够了。**每一个品牌的背后，都是隐藏着消费者对这个品牌内在的认知。如果App的使用体验与消费者的认知相符，那消费者大概率会一直使用。**如果消费者发现这个App的使用体验与认知不符，或者与自我设想中的比较类似，那可能大概率就不会留下。比如说打开今日头条App，你的预期是看下今天的天下新闻，但如果刷出来了很多搞笑段子，你可能大概率是不会留下的。

品牌的力量还体现在，一个成熟的品牌，是可以内化成为一个动词。用户在进行某种动作的时候，可能会第一时间就想到某个品牌。如果一个品牌可以做到这个程度，用户的留存一般都是会非常高的。比如搜索vs百度；发消息vs微信。其实就是品牌在消费者心目中的认知过于强烈了。

于是我们就拆解清楚了DAU的两个重要的影响因素，用户新增和留存。**一般意义上，用户新增量的增长是有一些术可以去追求的，短期内如果想砸钱可能也可以搞定。但是如果要把一个App真正的做起来，还是要思考用户应该怎么样留存下来，这才是一个App长久的发展之道。**

## 使用体验

接下来的两项我们合在一起说：**用户平均使用时长 × 单位时长广告的曝光次数**

用户的平均使用时长，很明显是一个推荐算法可以重点优化的指标。其实从经验看，用户的使用时长和用户的留存在很大程度上是正相关的——你觉得一个App好用了，你每天使用它的时长就会更长，同样的后面几天打开它的概率也就会越大。

单位时长广告的曝光次数，则是一个综合的产品决策了，因为这涉及到广告位的多少。广告位多了，用户不喜欢，用户的留存就会降低；广告位少了，收入不达标，不能最大化公司的收入。这其实是一个损失和收入trade-off的结果。因为现在用户普遍比较反感的点是在视频或者文章中段插广告，除非是视频作者或者文章作者的刻意为之。所以从这个角度说，同时这个指标和推荐还是有一点关系：推荐出太长的内容，是会影响广告收入的。(比较内容比较短的视频App想到了什么？没错，就是抖音。这也是这个产品本身很成功的地方。)

所以我们其实也已经拆解出了推荐算法在建模的时候需要注意的一些目标了：
* 最大的目标是保证用户留存，当然这个前提内容分发足够精准
* 尽可能让用户在App停留的时间更长，同时要注意控制，不能为了追求太长，而减少广告曝光。
* 需要有一个好的分发机制，帮助那些不是那么知名的作者可以成长起来。

## 广告收入

最后的几项： **广告点击率× 转化率 × 客单价 × 广告分成。**

其实是广告算法主要考虑的问题，广告算法整体上和产品本身关联的就不是那么明显，更像是一个抽象好的技术问题。广告算法整体上我了解的并不多，这里只说一些我了解到的东西。

相对于推荐，广告是一个约束条件更多，优化目标更直接，更为技术的一个岗位。推荐与广告的核心诉求都是预估用户对某一个item是否满意。核心的目标都是做点击率预估。这也导致了推荐和广告整体的技术栈相似。此外，广告对于收入的贡献相对于推荐来说更加直接。推荐是通过优化点击率影响用户的使用时长或者留存来达到提升收入的目的，而广告优化点击率就可以直接影响最终的广告收入。所以，我个人觉得推荐更偏产品，广告更偏技术。

此外，个人总结一下有以下几点区别，具体是：

* 整体广告投放是有预算约束的(广告主的钱是有限制的)
* 广告主一般还会提一些要求，比如要投放到特定的人群上(比如投放到年轻女性上的化妆品广告)
* 广告主广告投放的周期相对来说比较短，比如双十一期间的广告可能只有几个小时
* 此外广告的计价体系也是千差万别，不同的计价体系下，需要关注的点也不一样

顺便说一句，每一个DAU能为App平均带来的收入，从统计意义上说是基本稳定的。有一个统计指标用来衡量这个值，叫做ARPU(Average Revenue Per User)，度量了一个App变现能力的高低。大家看上市公司财报可能会经常出现这个值。大家看某一个公司变现做的好不好，看这个值就可以了。

- - - -

如今我们再回过头来看这样一个变现的公式，可以清楚的看到UG(用户新增)、推荐(用户留存)、广告(变现)在其中的重大作用。

**广告收入 = DAU × 用户平均使用时长 × 单位时长广告的曝光次数 × 广告点击率× 转化率 × 客单价 × 广告分成**

**还有一点是，我们在学校里面，或者是学术领域关注的，NLP和CV的常见问题，在这个公式中其实并没有直接的体现出来，更多的是通过间接的方式和收入公式建立联系，比如作为NLP分类作为推荐模型的原始特征进行输入。这可能也是学校和工业界关注的问题有差别的重要原因。**

- - - -

除了广告变现之外，现在互联网公司也在尝试一些其他变现的方式：比如直播、会员等等，其中原理其实和广告是类似的。都是在一定用户群(DAU)的基础上，尽可能给用户找到他可能潜在喜欢的内容，留住他，然后再通过某种方式让他进行付费，转化成用户。大家可以按照类似的角度，思考一下。

比如现在大火的直播，大家可以思考一下直播应该从什么样的角度去建模，怎么样可以留住用户，而传统的信息流的推荐有什么异同。又怎么样可以鼓励用户多消费，应该采用什么样的策略。**如果能够给公司创造更大的价值，个人的发展的渠道和路径自然也是一路畅通。**

- - - -

## 成本

之前我们都一直在谈收入，我们再来谈一下成本。其实从一个公司的角度出发，凡是不能创造收入的成本，对于公司来说其实都是属于无用的成本，需要被干掉。

除了公司正常的人力成本之外，在对收入至关重要的三驾马车(UG、推荐、广告)中，UG相关的成本我们已经介绍过了，可以通过ROI进行度量策略的好坏。

推荐和广告这个方向，目前最大的成本肯定还是机器成本。所以现在一个研究的重要方向是，怎么样可以在模型效果保持不变的情况下，尽可能的减少机器成本。比较关键的就是进行模型的精简；以及对运算本身进行更进一步的优化。**而后者的巨大需求，也造就了现在搞AI基础设施的工程师极度紧俏的——假设你可以优化一个分布式计算CPU消耗仅为原来的40%，那就相当于是公司的机器成本可以变成原来的40%呀。**


## 总结

在商言商，如果想在公司取得更好的位置和级别，非常重要的一点是要为公司创造出更大的价值。如果想为公司创造出更大价值，就需要从全局的角度思考，公司当前的价值是由什么构成的，瓶颈在什么地方，我们能为这个瓶颈又能有什么样的贡献呢。
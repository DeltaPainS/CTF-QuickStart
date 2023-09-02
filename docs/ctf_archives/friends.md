---
comments: true

---
# CTFer档案馆
## List
- [ek1ng｜Hidden Gem](https://ek1ng.com/)
- [曾哥｜弱小和无知不是生存的障碍，傲慢才是！](https://blog.zgsec.cn/)
- [Steven Lynn's Blog｜Steven的个人博客](https://blog.stv.lol)

## Recent Post
### [渗透基本思路总结](https://www.ek1ng.com/Summary%20of%20penetration%20ideas.html)  
>by [ek1ng](https://ek1ng.com/), 2023-08-29

最近做了一阵子攻防相关的事，正好最近国护结束，做个总结，简单写一下渗透的基本思路（Check List）。不同的标题间内容并不完全独立，在实战中，比如先钓鱼获取到一台个人PC，但这台PC并不在办公网。而后通过收集个人PC的信息，能够登陆外网其他站点的后台，配合一个后台RCE进入办公网/生产网。这其中就有钓鱼，也有外网打点的部分。资产收集资产搜集通俗说就是“了解目标有什么东西”，讲究一个越全越好。路...
### [Telegram Instant View即时预览适配过程记录](https://blog.stv.lol/archives/72/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-08-27

Telegram有个即时预览的功能，可以以阅读格式的页面形式加载网页，减少加载不必要的内容Telegram自己的Blog，以及主流内容平台（比如wikipedia, Medium, 知乎都有人做了适配）但直到今天一番研究才知道适配工作要在instant view上面写规则，并且提交审核这个工作可以说基本上由用户维护，官方通过排名的方式来选择每个网站最好的Instant View模板，也有2017和...
### [英国铁路系统体验小结](https://blog.stv.lol/archives/67/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-08-27

今年暑假去了趟英国，在英国生活了半个月的时间打算分几篇文章简述一下一些感受这篇文章主要讲讲英国的铁路系统（包括地铁和火车）文章偏体验向，可能比较流水账，想到哪写到哪概述因为起步时间早，英国铁路系统相当发达，早在19世纪就已经开始建成世界第一条地铁线路，后续又建了许多线路并不断完善城市铁路网络在伦敦市区，火车与地铁共用线路，可以凭oyster进站上下车，速度也与地铁速度一致，离开共用线路之后恢复至正...
### [Java RMI 攻击梳理总结](https://www.ek1ng.com/java-rmi-attack.html)  
>by [ek1ng](https://ek1ng.com/), 2023-07-26

RMI 是什么定义RMI（Remote Method Invocation）是远程方法调用，类似RPC（Remote Procedure Calls）。RPC是打包和传送数据结构，而在Java中，通常传递一个完整的对象，包含数据和操作数据的方法。通过RMI，能够让客户端JVM上的对象，像调用本地对象一样调用服务端JVM上的对象。RMI引入了 Stubs（客户端存根）和 Skeletons（服务端骨...
### [重学 Java 反射机制](https://www.ek1ng.com/java-reflect-learning.html)  
>by [ek1ng](https://ek1ng.com/), 2023-07-25

近期跟一些java的最新漏洞，发现自己的语言基础太差了，跟着p牛的java安全漫谈重新学一下反射，p牛的文章确实是讲复杂的东西讲的浅显易懂。反射的定义对象可以通过反射获取对应的类，类可以通过反射获取所有方法，拿到的方法可以调用，这种机制就是反射。反射机制在安全方面的意义例如我们要完成RCE，但代码中绝大多数时候并没有Runtime，ProcessBuilder等常见的用于命令执行的类来让我们调用。...
### [java-sec-code 代码审计靶场题解](https://www.ek1ng.com/java-sec-code.html)  
>by [ek1ng](https://ek1ng.com/), 2023-07-20

这个靶场包含了各类基本漏洞在java语言上的场景以及java安全特有的JNDI注入，反序列化，表达式注入等等，并且给出了相关的利用手段和修复方案。java-sec-code搭建环境可以用Docker搭建，不过想了想不太熟练java的包管理和web server部署这一套，并且本地起相比于容器也方便调试，于是决定本地起一份。由于我是archlinux，包管理安装的都是最新的jdk版本，靶场的jdk版...
### [当无回显RCE碰上Win服务器](https://blog.zgsec.cn/index.php/archives/306/)  
>by [曾哥](https://blog.zgsec.cn/), 2023-07-17

0# 概述在日常的渗透过程中，总会碰到一些RCE漏洞，无回显的RCE漏洞更是家常便饭。对于无回显的漏洞利用，网上有不少文章，但我看了半天，都是Linux系统的当无回显RCE漏洞碰上Win服务器，我们又该何去何从呢？故创建本文做个记录本人才疏学浅，如本人有所疏漏，也望各位师傅指点一番1# 无回显上线C2遇到无回显的RCE漏洞，上线C2是不二之选，但这部分并不是今天的重点：上传C2到服务器一般有以下操...
### [CrewCTF 2023 Web Writeup](https://www.ek1ng.com/2023CrewCTFWP.html)  
>by [ek1ng](https://ek1ng.com/), 2023-07-14

环境还在，赛后看看题，一共四道Web，都挺有意思的。sequence_galleryDo you like sequences?http://sequence-gallery.chal.crewc.tf:8080/ 123456789101112131415sequence = request.args.get('sequence', None)if sequence is None:    re...
### [旅行日志：无锡&amp;苏州小记](https://blog.stv.lol/archives/61/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-07-09

在苏北那个鬼地方关了两年多，尤其之前一直在被各种考试折腾，终于放暑假了，于是临时起意去长三角几个城市玩两天一个人出行最大的好处在于自由度，可以想到哪里就去哪里以及，和朋友们面基！这篇文章想到哪写哪，因此全文可能看起来比较流水账多图警告Day1 无锡说起来以前经常从无锡的高速或者火车站经过，但从来没有真正到过无锡，所以这一次来算是第一次玩先说下无锡的印象吧，个人觉得无锡这个城市既现代化又不怎么现代化...
### [群晖NAS折腾笔记：FRP内网穿透&amp;FTP](https://blog.stv.lol/archives/60/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-07-06

在今年年初我购入了j4125工控机目前这台的配置是exsi主系统，虚拟机中的子系统是Windows 10，OpenWRT，群晖，也就是NAS+软路由+主机的三合一配置其实在这篇文章之前应该还有组装篇和系统安装篇，之前一直没写，先鸽着FRP内网穿透配置篇考虑到国内很难买到便宜的大带宽服务器，而用国外的服务器做穿透也很难满足速度和延迟要求，再加上服务端配置可能比较困难，所以我直接使用的SakuraFr...
### [渗透必备：使用Proxifier玩转代理](https://blog.zgsec.cn/index.php/archives/278/)  
>by [曾哥](https://blog.zgsec.cn/), 2023-07-02

0# 概述在日常的渗透过程中，不管是前期的外部打点还是后渗透，代理总是绕不开的话题。在前期的外部打点过程中，扫描和渗透测试会不断受到WAF的拦截，需要不停的更换IP进行扫描和渗透测试；而在后期的后渗透过程中，通过Frp和Nps等等工具从入口点出网之后，也需要对接代理进入目标内网进行内网渗透。本文内容是我个人自己摸索出来的，也有可能别的师傅也有类似的方法哈哈。1# Proxifier介绍本文我们需要...
### [中信银行美国运通借记卡评测](https://blog.stv.lol/archives/59/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-06-30

最近开的卡有点多...如上篇介绍广发银行的美国运通卡所述，美国运通的人民币借记卡有免换汇的优点，目前体验下来中信银行的这张美国运通借记卡也完全一致，虽然卡面上写了member，但并没有给什么权益，毕竟这只是一张借记卡而已建议先阅读广发这篇[post cid="45" /]这张卡是5月份推出的，时至今日仍然未出现在美国运通中国官网上结论先说在前面：如果你已经有一张美国运通卡或者Mastercard/...
### [最好的年华献给最糟糕的时光：我两年的大学生活](https://blog.stv.lol/archives/58/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-06-29

不知不觉大学都两年下来了，挺快的在上大学之前，我从未仔细思考过自己真正需要什么，仅仅被填鸭式的中式教育所驱使，也就是按照大众的思路：上个好小学->考个好初中->考个号高中->考个好大学->考个研究生->有个好工作大部分人似乎从未想过这样做的意义，似乎这样的一套人生轨迹已经成为了亘古不变的人类社会规律，就像是西西弗斯推着巨石，做着永无尽头而又徒劳无功的任务；也从来没有人指出另外的道路，似乎背离这条道...
### [云原生安全分享会材料](https://www.ek1ng.com/cloudsecurity.html)  
>by [ek1ng](https://ek1ng.com/), 2023-06-28

这是一篇用于给协会小学弟们分享的文章，粗略从各个角度讲了一讲，有任何问题都欢迎联系我交流，email：ek1ng@qq.com。基础知识🧀在开始之前，你需要能够基本掌握Docker和Kubernetes的使用。基本使用推荐看官方文档，配合一些教程动手尝试。https://www.docker.com/Docker 能区分镜像/容器，能基本使用命令，能写Dockerfile，粗略了解原理即可。htt...
### [Cloudcone Nexus CDN 踩坑&amp;简评](https://blog.stv.lol/archives/57/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-06-24

Cloudcone出了一个$4.5/年的CDN，一个月5GB的流量，国内能直连台湾中华电信的节点，体验不错，并且有waf防护，正好把博客的小站升级一下购买链接Hashtag 2023 CDN – 15 GB月流量$4.5/年购买链接Hashtag 2023 CDN – 210 GB月流量$8.99/年购买链接Hashtag 2023 CDN – 320 GB月流量$17.99/年购买链接Hasht...
### [SQL注入恶劣环境之可执行文件上传骚姿势](https://blog.zgsec.cn/index.php/archives/258/)  
>by [曾哥](https://blog.zgsec.cn/), 2023-06-01

0# 概述在前期Web打点成功获得对应权限后，就进入了后渗透（提权、内网渗透、域渗透）的阶段，但是在有些时候，总会出现各种各样奇怪的情况，在此也分享一些经验出来。最近在打红队外援碰到了一个站点存在SQL注入，于是尝试用SqlMap对网站进行注入，发现注入成功，但由此也引发了一系列问题。可能你看完本篇文章，会觉得原理其实很简单。但试问你自己，在面对以下情况的时候，能想到通过这样的手法达成你的目的吗？...
### [【重要通知】域名更换通知](https://blog.stv.lol/archives/55/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-05-29

因为原有域名[bebebe.be]即将到期且续费困难问题，本站即将停用该域名并更换为[blog.stv.lol]为了配合新域名，本站原名[哔哔哔哔]更名为[Steven Lynn's Blog]，stv即Steven的缩写具体更换内容如下内容原现域名bebebe.beblog.stv.lol站点名称哔哔哔哔Steven Lynn's Blog图标https://s2.loli.net/2022/1...
### [AI绘画非技术性入门：Midjourney与Stable Diffusion上手](https://blog.stv.lol/archives/54/)  
>by [Steven Lynn's Blog](https://blog.stv.lol), 2023-05-27

写在开头众多AI绘画工具的问世和发展已经有一段时间了。笔者虽然并非AI绘画的最早一批玩家，但也自认为是比较早入门的。最早的接触是在2022年夏OpenAI Dall-e的新模型发布后在官网体验到的。在2022年10月底，也就是NovelAI的二次元模型泄露后，AI绘图开始走向平民化，我也是在11月初左右开始正式接触这个领域。其实很早以前，大概在2022年12月就想写这篇文章了。之所以拖到今天才开始...
### [阿里云 BrokenSesame RCE漏洞分析](https://www.ek1ng.com/BrokenSesame.html)  
>by [ek1ng](https://ek1ng.com/), 2023-05-12

学习了Wiz团队发表的文章 https://www.wiz.io/blog/brokensesame-accidental-write-permissions-to-private-registry-allowed-potential-r，有很多巧妙的利用方法可以学习Wiz Research在文章中披露了被命名为BrokenSesame的一系列阿里云数据库服务漏洞，会导致未授权访问阿里云客户的Po...
### [2023西湖论剑·数字安全大会有感](https://blog.zgsec.cn/index.php/archives/214/)  
>by [曾哥](https://blog.zgsec.cn/), 2023-05-12

前言今年终于抽空去参加西湖论剑·数字安全大会了，参加后感触颇多，回来的路上就想着写一篇文章来分享一下此行的收获。但苦于最近事务繁多，直到今日才有闲暇之时来落笔本文，各位师傅见谅。本来我们有四个人一块同行的，我和皓哥、垚垚以及俊哥，可惜中途由于私事，俊哥中途离开了我们回老家了。这是我们三个在西湖论剑的现场合影：PS：横跨整个杭州来参会，脚都要走废了哈哈注明：本文图片比较多，可以往下拉跳过图片，看一下...
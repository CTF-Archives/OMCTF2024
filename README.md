# OMCTF 2024

2024 高校网络安全管理运维赛 附件归档 OMCTF2024（operation and maintenance）

## Misc - 签到

> 点击下面的链接下载附件。在 GIF 图片中提取出 Flag，然后将 Flag 输入到下面的文本框即可得分。
>
> 本比赛的统一 Flag 格式为 flag{...}，Flag 区分大小写，所有字符均为可打印 ASCII 字符。本题的 Flag 是在英文中有意义的内容，且所有字母均为小写。

## Misc - 钓鱼邮件识别

> 你是 Foobar 大学的安全分析师。一位名叫张三的员工报告了一封可疑的邮件，并将其提供给你进行分析。你的任务是仔细检查这封邮件，识别潜在的钓鱼指标，找出表明这是一次钓鱼尝试的线索。
>
> 可疑邮件以 EML 文件的形式提供，请查看附件。

## Misc - easyshell

> 网站被攻击了！你能从流量文件中分析出被偷走了什么数据么？

## Misc - SecretDB

> Find secret from DB.

## Misc - Gateway

> 小张买了一个新的网关，并暴露到了外网，由于默认口令的原因，黑客很快登录了系统并重置了密码，这个黑客甚至在他的电脑上留下了这个网站的部分代码，你能帮他找到密码并解密成功吗？

## Misc - zip

> Alice 把 flag 用你的 token 压缩并加密成了一个 zip 压缩包，并且希望你提供 flag 来解压这个压缩包。
>
> 如果解压成功， Alice 就会告诉你 flag 的内容，但好像 Alice 的代码实现有些问题？

## Misc - Apache

> Apache 会有什么问题？

本题实际上有两个容器，附上扒下来的 Python 源码

## Misc - f or r

> Got a new KB update from Macrohard. (提交 flag 时请删除所有空格)

## Web - phpsql

> 你能变成管理员么？

## Web - pyssrf

> 嗷，我的上帝，怎么还会有人在用 python:3.7.1。flag 文件位置：/flag

## Web - Messy Mongo

> 这是一个关于大学生小华编程奋斗历程的故事。
>
> 小华是个热爱编程的大一新生, 她对编程课程充满热情。然而当老师布置了基于 MongoDB 的 TODO 网站大作业时, 她却感到了前所未有的挑战。
>
> 一开始, 小华对 MongoDB 的概念有些陌生, 她在网上查阅了大量的教程和文档。通过不懈的努力, 她逐步掌握了 MongoDB 的基本操作, 并开始着手设计网站的整体架构。
>
> 小华决定先从设计数据库开始入手。她构思了一个简单但实用的 document schema, 将 TODO 任务项目的各种属性如标题、内容、完成状态等进行了细致的规划。在设计过程中, 她也意识到了数据安全性的重要性, 因此决定采取一些措施来加强网站的安全性。
>
> 通过查阅资料, 小华了解到可以在 MongoDB 中设置 document validation, 从而限制插入和更新数据时必须符合预定义的 schema 结构。这不仅可以确保数据的完整性和一致性, 而且还能防止攻击者注入恶意数据。于是, 她在自己设计的 TODO document schema 中添加了相应的 validation 规则。
>
> 数据库的设计工作完成后, 小华开始着手网站前端和后端的开发。虽然过程中遇到了不少困难和挫折, 但她都一一克服了, 并且渐渐掌握了使用 MongoDB 进行数据存取的技巧。
>
> 就在她以为可以顺利完成这个大作业时, 一个新的问题突然出现了。在进行功能测试时, 她发现从前端发来的某些特殊格式的输入数据, 竟然可以逃过 MongoDB 的 document validation 检查, 并成功写入数据库。小华意识到这是一个严重的安全隐患, 如果网站上线后被攻击者发现并加以利用, 那将造成无法挽回的灾难。
>
> 经过一番仔细排查, 小华终于发现了问题所在。原来是由于她在前端对用户输入数据的过滤不够严格, 导致攻击者可以构造出不符合预期格式的数据。她当机立断地对前端代码进行了重构, 增加了更为严格的数据验证逻辑。
>
> 在确保前后端数据交互的安全性后, 小华终于可以放下心中的一块大石, 将注意力集中在完善其他功能上了。经过将近一个学期的努力, 她终于完成了这个 TODO 网站, 在演示答辩时赢得了老师和同学的赞许。
>
> 这个大作业不仅锻炼了小华的编程能力, 更重要的是让她认识到了网络安全的重要性。她深刻地体会到, 要构建一个真正安全可靠的应用系统, 不能只停留在单一的技术层面, 而必须从架构、设计、实现的各个环节都予以足够的重视。这次宝贵的经历必将成为小华日后在编程道路上持续奋斗的强大动力。
>
> 当然，以上都是由 Claude 杜撰的情节，而你的工作则是找出源码中的隐藏问题。

## Web - JustXSS

### 简述

在这个充满各种现代 Web 安全挑战的时代，我们时常被各种复杂的攻击和防御手段所困扰。然而，有时候，回归基础、专注于最本质的攻击方式，反而能够带来更深入的理解和启示。JustXSS 就是这样一道专注于跨站脚本攻击（Cross-Site Scripting, XSS）的题目，旨在让你在纯净的环境中，返璞归真，重新感受 XSS 的魅力与威力。

### 背景

随着 Web 应用的不断发展，XSS 攻击作为 Web 安全领域最基础也最常见的攻击方式之一，始终保持着其独特的地位。然而，随着现代 Web 框架和防御机制的不断完善，许多开发者往往忽视了对 XSS 攻击的防范。JustXSS 题目将带你进入一个简化的 Web 环境，让你专注于 XSS 攻击的本质，从而更好地理解其原理和防范方法。
目标

你的任务是在给定的 Web 应用中，通过构造恶意的输入数据，触发 XSS 攻击，并成功执行你植入的 JavaScript 代码。题目将提供一个包含 XSS 漏洞的 Web 页面，你需要利用这个漏洞，实现诸如窃取用户 Cookie、篡改页面内容等恶意操作。

### 挑战

发现漏洞：首先，你需要仔细分析提供的 Web 页面，找到其中存在的 XSS 漏洞。这可能需要你具备一定的 Web 开发基础和安全意识。 构造攻击载荷：一旦你发现了漏洞，就需要构造合适的攻击载荷。你需要确保你的载荷能够绕过任何可能存在的输入过滤或编码机制，并成功地在目标用户的浏览器中执行。 执行恶意操作：当你的载荷成功执行后，你就可以开始执行各种恶意操作了。你可以尝试窃取用户的 Cookie、篡改页面内容、重定向用户到其他恶意网站等。

### 提示

- 专注于 XSS 攻击的基本原理和常见手法，不要试图使用复杂的攻击技巧或工具。
- 仔细阅读题目提供的背景信息和提示，它们可能会为你提供一些有用的线索。
- 尝试从多个角度思考问题，不要局限于一种解决方案。

### 注意事项

- 本题目仅用于学习和研究目的，请勿在未经授权的情况下对任何网站或系统进行攻击。
- 在进行攻击测试时，请确保你的行为符合相关法律法规和道德规范。

## Web - expr

> 请获得主机根目录下的flag文件内容

## Web - fileit

> flag保存在根目录的flag文件中

## Reverse - easyre

> flag被奇怪编码过了，试试看能否还原出原文？

## Reverse - babyre

> 真正的程序似乎被藏起来了，你能找到flag吗？

## Pwn - Login

> 在端口扫描结果中，你发现了一个奇怪的开放端口，可以通过ncat进行交互。然而你并没有找到任何相关信息，你可以破解它嘛？
>
> 在一片神秘的网络上，有一座被称为“赛博之城”的地方。这座城市的居民都是一些数字生命体，他们生活在一个由0和1构成的世界里。赛博之城有着严密的防御系统，任何试图闯入的非法分子都会被毫不留情地拒绝。然而，这座城市里隐藏着一个传说，那就是在城市的深处，有一个神秘的宝藏，得到它的人将能获得巨大的力量。
>
> 作为一名赛博淘金者，你一直在寻找传说中的赛博之城。经过长时间的努力，你终于找到了这座城市的入口。然而，在你试图进入时，却被城市的防御系统发现并拒绝。你不甘心就此放弃，于是决定寻找其他入口。
>
> 在一次偶然的端口扫描中，你发现了一个奇怪的开放端口。端口上有一个登录入口，似乎与赛博之城的某个后台系统有关，但却没有任何相关信息。你觉得这是一个机会，于是决定尝试破解这个端口……

## Pwn - babypwn

> 一个很baby的pwn

## Algorithm - babyai

> flag被藏在书里了，幸好你找到了一台找flag的机器人。
>
> 这台机器人被训练成朝着flag所在的方向前进。
>
> 你能开着机器人找到flag吗？

## Algorithm - secretbit

> 我的flag被使用如下脚本加密了，请帮我还原出flag内容

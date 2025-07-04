# Python 潮流周刊#50：我最喜欢的 Python 3.13 新特性！

pubDate: 2024-05-12

你好，我是猫哥。这里每周分享优质的 Python、AI 及通用技术内容，大部分为英文。另有[电报频道](https://t.me/pythontrendingweekly)作为副刊，补充发布更加丰富的资讯，欢迎关注。

本期分享了 12 篇文章，11 个开源项目，2 则音视频，全文 2200 字。

## 🦄文章&教程

1、[我最喜欢的 Python 3.13 新特性](https://treyhunner.com/2024/05/my-favorite-python-3-dot-13-feature/)

Python 3.13 在进入功能冻结期前，添加了一个全新的 REPL，作者表示这是 Python 3.13 中他最喜欢的特性。新的 REPL 确实让人眼前一亮：彩色提示、下一行自动缩进、tab 自动缩进 4 格、exit 和 help 不用再加括号、支持块级历史记录、支持粘贴代码块……这些新功能也是我一直想要的，现在终于要支持了。遗憾的是，它还不支持 Windows 系统！

2、[Python 3.13 新功能盘点介绍](https://iscinumpy.dev/post/python-313/)

Python 3.13 beta 1 版本已发布，改动内容真不少呢，文章做了一个简单盘点：改进的 REPL、自由线程（无 GIL Python）、JIT 编译器、python -m random 生成随机数、对 iOS 的 tier 3 级支持，等等等。（附：所有变更内容，详见官方文档 [What's New In Python 3.13](https://docs.python.org/zh-cn/3.13/whatsnew/3.13.html)）

3、[Python Asyncio 工作原理：从零实现一个简化版 Asyncio](https://jacobpadilla.com/articles/recreating-asyncio)

作者用生成器、async和await关键字，逐步从零构建，成功模拟出asyncio的事件循环和任务调度机制，可加深你对asyncio内部工作原理的理解。（附：文章的[中文翻译](https://juejin.cn/post/7366945260792447014)）

4、[友好的 Python：封装和复用](https://frostming.com/2024/friendly-python-reuse/)

这是一篇标题友好的无情吐槽文，被吐槽的是火山引擎的 TTS 接口及其 SDK 设计。作者详细分析了对方代码的问题，给出了改进建议和原则，最后还贴心给出了 62 行的改进版本，远胜原始的近 500 行的版本。

5、[零基础入门 Python 文件处理篇——实现一个简单的文件搜索引擎](https://juejin.cn/post/7363454217191686181)

文章收集了很多 Python 文件操作的知识和代码片段，涉及基础和进阶的各类文件操作，可以查漏补缺。最后还演示了从给定目录下模糊搜索一个文件的代码。

6、[用 HTMX 和 Django 开发一个 Connect Four 游戏](https://www.photondesigner.com/articles/connect4-htmx)

一个用 Django + HTMX 开发 Web 小游戏（Connect Four）的简单教程。通过游戏项目来学习编程，应该是效果不错的方式。

7、[用 wxPython 开发一个简单的计算器](https://www.pythonpapers.com/p/creating-a-calculator-with-wxpython)

计算器是很好的用于练习 Python GUI 编程的项目，类似的教程在网上有不少，但是像这篇那么详细介绍每一段代码的应该不多。

8、[学生在入门数据科学时常犯的错误](https://austinhenley.com/blog/datasciencemistakes.html)

在入门数据科学时，哪些错误时常会发生？这篇论文对 500 多份样本作定性分析，指出了这几类错误：逻辑错误、语义错误、次优编码、对语言和环境的误解。

9、[使用“不安全的 Python”加速 Numpy 代码 100 倍](https://yosefk.com/blog/a-100x-speedup-with-unsafe-python.html)

“Unsafe Python“是指可能导致安全风险或内存安全问题的技术。作者使用pygame 和OpenCV 来处理图像缩放任务，发现性能差距很大，原因是由numpy 数组的内存布局（strides）引起的，最后通过优化内存访问模式来提升性能。

10、[Python 字典详细的历史演变过程](https://discuss.python.org/t/developing-a-detailed-historical-understanding-of-python-dict-implementations/52618)

这是在 Python Discuss 论坛上的一篇帖子，作者想梳理字典的技术细节和历史演变，但是发现字典在不同版本的插槽数、扩容机制和初始大小等方面差别很大。

11、[重新发明 Python notebook 的经验教训](https://marimo.io/blog/lessons-learned)

marimo 是作者开发的一款 notebook 产品，是 Jupyter notebook 的竞品，已经被斯坦福大学和贝莱德等机构使用。文章介绍了其三项设计原则：可重现、可维护、多用途，为什么要采用这些设计，以及在实现的过程中学到的几点经验教训。

12、[Python 软件基金会新闻：2022 和 2023 资助计划的透明度报告](https://pyfound.blogspot.com/2024/05/psf-grants-program-2022-2023.html)

PSF 发布了前两年对 Python 社区的资助计划的透明度报告。我们周刊第 30 期分享过泛非 Python 社区的一封公开信，就是质疑 PSF 的资助计划。报告公布了各项支出、趋势、百分比等数据，特别分享了关于非洲早年的几起资助。

## 🐿️项目&资源

1、[pywinassistant：用自然语言控制 Windows 用户界面](https://github.com/a-real-ai/pywinassistant)

这是一个大动作模型（Large Action Model），使用自然语言操作 Windows 系统。目前支持所有通用的 win32api 应用。

2、[chinese-calendar：判断一天是不是法定节假日/工作日](https://github.com/LKI/chinese-calendar)

判断某年某月某一天是不是工作日/节假日，支持 2004年 至 2024年。（附：另一个同名的项目[chinese-calendar](https://github.com/overtrue/chinese-calendar)，是个农历/阴历与阳历/公历的转换与查询工具）

3、[Oven：探索 Python PyPI 包](https://pyoven.org/)

支持搜索和查看 PyPI 上的软件包，支持查看 pip/pdm/rye/poetry 安装命令，支持查看每周下载量和趋势图。

![](https://img.pythoncat.top/2024-05-11_pyoven.png)

4、[tetos：适用于多种 TTS 服务的统一接口](https://github.com/frostming/tetos)

使用一套统一的接口来对接不同的文本转语音（TTS）服务商，已支持 Edge-TTS、OpenAI TTS、Azure TTS、Google TTS、火杀引擎、百度 TTS、Minimax TTS。

5、[relax-py：又一个 Python Web 框架](https://github.com/crpier/relax-py)

Python Web 开发框架，基于 Starlette + htmx + tailwindcss，具有热模块替换（HMR）、基于路径函数的 URL 定位器、依赖注入等特性。

6、[哈佛大学 2024 年 CS50 线上课程](https://cs50.harvard.edu/x/2024/)

哈佛大学的 CS50 是一个计算机科学入门课程，有 11 周课时安排，免费提供所有学习资源，可颁发课程证书。今年的变化是引入了由 ChatGPT 支持的对话机器人，可帮助回答与课程相关的问题。

![](https://img.pythoncat.top/2024-05-10_CS50.png)

7、[portr：专为团队设计的开源的 ngrok 替代方案](https://github.com/amalshaji/portr)

Portr 是一种隧道解决方案，可向互联网公开本地 http、tcp 和 websocket 连接。它利用 SSH 远程端口转发来保证隧道连接的安全性。（star 2K）

8、[py-compress-compare：对比分析 zlib、LZ4、Brotli 和 Zstandard](https://github.com/dhilipsiva/py-compress-compare)

这个项目对四个流行的 Python 压缩库（zlib、LZ4、Brotli 和 Zstandard）进行对比，衡量了压缩比、压缩时间、解压时间等指标。

9、[pyspread：用 Python 开发的电子表格，可支持 Python 代码](https://pyspread.gitlab.io/)

使用 Python 开发的 Excel，单元格中支持 Python 表达式，并且每个单元格返回的都是一个 Python 对象。可从单元格访问 Python 模块，包括 Numpy；支持导出 CSV、SVG 和 PDF 等格式。

![pyspread界面](https://img.pythoncat.top/pyspread.png)

10、[PgQueuer：基于 PostgreSQL 的任务队列库](https://github.com/janbjorge/PgQueuer)

一个极简的 Python 任务队列库，使用 PostgreSQL 的 LISTEN/NOTIFY 来管理任务作业，使用 pg 的FOR UPDATE SKIP LOCKED 实现可靠的并发处理。

11、[你用人工智能做过的最实用的事情是什么？](https://www.reddit.com/r/ArtificialInteligence/comments/1ceaftk/whats_the_most_practical_thing_you_have_done_with/)

除了用作图像生成和简单的问答，你还用 AI 做过什么有用的事情？这是 Reddit 的热门帖子，可以看看别人都开发过什么项目，从而找找个人项目的创意。

## 🐢播客&视频

1、[core.py](http://core.py/)[ Ep 10：开发者聊 Python 3.13 的 REPL](https://podcasters.spotify.com/pod/show/corepy/episodes/Episode-10-The-Interactive-REPL-e2j788i/a-ab7uiak)

Pablo Galindo 和 Łukasz Langa 开发了 Python 3.13 中新的 REPL，他们在播客中聊了开发这个特性的故事，也分享了 CPython 最近改动的一些特性，比如新的 JIT 和 Python 对 iOS 的支持等。

2、[The Python Show 40 - 与 Antonio Cuni 一起聊开源开发](https://www.pythonshow.com/p/40-open-source-development-with-antonio)

这期播客的嘉宾是 PyScript、pdb++、pypy、HPy 和 SPy 等开源项目的贡献者，播客聊了参与开源开发的相关话题。


# 南京邮电大学本科毕业设计Latex模板

## 小故事

- 又快到一年一度的毕业季了，在此真是无比怀念。Mark一下，此时是2022/3/1。

- 但是大家用Word写论文会增加不少烦恼，参考文献问题首当其冲，再其次就是格式，让好多人头疼无比

- 很多人觉得Latex很难上手，其实不是（手动狗头）。最大的问题还是没有合适的模板。前人栽树，后人乘凉。2021年的春天，我在github上看到了[`imguozr`](https://github.com/imguozr)的[`NJUPThesis-Bachelor`](https://github.com/imguozr/NJUPThesis-Bachelor)以及另一位hxd修改过的[`NJUPThesis-Bachelor`](https://github.com/lemoxiao/NJUPThesis-Scholar)。看起来我有希望了是不是，有现成模板，不用Latex天理不容！（狗头保命）

- 但是我发现了问题，这些模板和官方的word出来的效果差太多了呀？这咋整？这个.cls文件已经被修改的m都不认识了，还没有注释，这……

- 算了，我从头改一遍吧……（当时哪来的勇气？梁静茹也不敢啊。。。）

- 依然可能有小问题，但总体比之前好很多，欢迎大家使用并提出建议。

## 介绍
本模板是南京邮电大学本科生(理工艺教类)毕业设计的Latex模板，该模板由[`NJUPThesis-Bachelor`](https://github.com/imguozr/NJUPThesis-Bachelor) 以及[`lemoxiao`](https://github.com/lemoxiao)修改过的[`NJUPThesis-Bachelor`](https://github.com/lemoxiao/NJUPThesis-Scholar)演化而来，并做了大量的修改工作和完善工作。

## 核心特征

- 使用了GBT-7714标准引用格式，经过我的研究，在我以上提到的模板中，其参考文献格式是最大的问题。经过对教务处给出的Word版本的模板进行研究，我发现其与GBT-7714模板高度一致，有理由认为应该就是GBT-7714。因此在模板中我使用了GBT7714引用格式。

- 修正了封面不在中间的问题

- 修改了页面参数，包括页边距、行距、段间距，页眉、页尾等等，和官方Word保持一致。

- 修改了结束语、致谢、参考文献的标题格式，修改了附录的格式。

- 修复了图注和表标题后面没有空格的问题。

- 修复了公式编号问题。

- 修改了原创性声明的格式，与官方保持一致。

- 其它大量的细节优化和 模板文件(`.cls`)注释添加

## 运行环境

1. 感觉毕竟是毕业论文，用overleaf显得有些草率，还是建议在本地编辑和编译。
2. 对于 `Windows` 系统，直接安装 `TeX Live` ，编辑器推荐使用`TeXstudio`。
3. `MacOS`经过[`Leo Y Chen`](https://github.com/xsro)的测试基本无问题，后续欢迎大家测试反馈。
4. [`Leo Y Chen`](https://github.com/xsro)提供了`vscode`的latex编译配置文件，存放在`.vscode/`文件夹中，由于本人暂不使用`vscode`，大家自行测试。

## 编译过程

带参考文献的中文文档，一般进行以下四次编译：

`XeLaTeX` -> `BibTeX` -> `XeLaTeX` -> `XeLaTeX`

一般来说我们最常用的是`TeXstudio`，在里面的选项->设置->构建中可以自己编写编译链。
## 使用指南

- `main.tex`: 这是tex源文件，我在里面填充了示例，可以对照生成的 `main.pdf` 熟悉代码。
- `reference.bib`: 论文的参考文献库。
- `./pic`: 将图片放入该文件夹，图片支持常规的格式如`eps`, `jpg`, `png` , `pdf`, `pdf`文件可以编译得更快。

## 字数统计 摘自：[`NJUPThesis-Bachelor`](https://github.com/imguozr/NJUPThesis-Bachelor)

1. 在命令行中使用 `texcount your-tex-file-name.tex` 命令进行统计。
2. 对生成的 PDF 文件进行统计。

## 已知问题

1. ~~目前来看唯一的缺陷可能是当时编写时比较急促，自身水平又比较差，在一些标题和题注的格式上，为了和官方Word模板几乎相同，我在里面加了一些空格或是间隔，本身是不推荐大家这样修改模板的，会造成在正文文段中引用时也出现空格和间隔。~~目前此问题已由[`Leo Y Chen`](https://github.com/xsro)解决。暂时无问题，欢迎大家反馈。
2. everypage的功能已经被官方支持所以不再需要这个包，所以这个包会警告。参见[ref](https://stackoverflow.com/questions/64921954/how-to-solve-latex-package-warning-for-everypage)

## Q&A

由于本人水平所限，如果有问题，欢迎大家提出issue，也欢迎解决后提`pull request`。

2021年我用这个模板撰写了我自己的毕业论文，没有任何问题，效果不错。我感觉每年官方的Word模板变动一般不会很大，所以大家修修补补还是可以用的。

如果觉得好用，你可以在致谢部分留下**本论文采用基于 LaTeX 的南京邮电大学本科论文模版编写**，欢迎附上本GitHub repo的链接。

## 贡献者名单
- [`dhiyu`](https://github.com/dhiyu)(Owner)
- [`Leo Y Chen`](https://github.com/xsro)(Contributer)

## 参考项目
- [`imguozr`](https://github.com/imguozr)的[`NJUPThesis-Bachelor`](https://github.com/imguozr/NJUPThesis-Bachelor)
- [`lemoxiao`](https://github.com/lemoxiao)的[`NJUPThesis-Bachelor`](https://github.com/lemoxiao/NJUPThesis-Scholar)

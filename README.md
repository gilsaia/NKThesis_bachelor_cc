# NKThesis_bachlor_cc
南开大学本科生毕业论文Latex模板(计算机、网安版本)

从[南开大学研究生论文模板](https://github.com/NewFuture/NKThesis)修改而来，但改动很大，除了模板文本保留以外，样式可以认为进行了全部重写

我个人比较厌恶Word排版，本想找一个毕设模板来直接使用，但找来找去发现并没有找到很好的南开大学本科生毕设模板，所以才产生了自己写一份的想法

在模板中并没有很多的可选设置，一方面是我确实没有充足的时间设计多套模板，另一方面我认为毕设模板所固定的绝大部分样式都是有严格要求的，应该不会进行很大改动
## 模板来源
[南开大学研究生（博士生）毕业论文LaTeX模板](https://github.com/NewFuture/NKThesis)

thanks to @darfux， @NewFuture

## Overleaf使用
经简单尝试目前版本可在overleaf使用 直接将整个项目打包之后将压缩包上传到Overleaf项目中即可 **之后将项目编译器切换为xelatex即可使用**

## 注意事项
- 除了需要安装`latex`环境以外，模板中使用的代码高亮宏包`minted`需要`python`环境以及`python`包`pygments`
- 目前的毕设标准存在冲突，主要参考的是在~~20年新发布的[南开大学本科毕业论文（设计）指导手册](https://cc.nankai.edu.cn/2020/1119/c13295a318941/page.htm)~~ **注意 指导手册中样例格式存在问题 目前尽量以文字描述为准**，如果有什么确定存在问题的样式非常欢迎提Issue讨论或提pr修改
- 目前找到的冲突项包括
  - 各级标题字号
  - 列表项编号
  - 封面字号
  - 封面及部分填充内容字体
## 目前存在的问题
- 开篇的封面以及声明，我尽量做到模仿手册中的模样，但很难做到一分不差的还原，如果使用者介意可以不使用模板的封面声明留到最后再与标准封面声明拼接
- 附录样式未调整完善
- 脚注带圈数字不美观
## 编写

### 编译方式
`xelatex`(Tex编译)+`biber`(参考文献编译)

#### 编译环境

我使用的是`TexLive2020`环境，在`VScode+Latex-Workshop`下编译，使用`xelatex`以及`biber`

#### 手动编译:

```
xelatex main
biber main
xelatex main
xelatex main
```

### 推荐编辑器和工具

基本要求: 自动补全，语法高亮，错误提示,实时预览,光标同步

* [VS code](https://code.visualstudio.com/) + [LaTeX-Workshop插件](https://github.com/James-Yu/LaTeX-Workshop)
* [sublime](https://www.sublimetext.com/) + [LatexTools插件](https://github.com/SublimeText/LaTeXTools) +[Sumatra pdf](https://www.sumatrapdfreader.org/download-free-pdf-viewer.html)

## 说明

### 文件
* [main.tex](main.tex)模板入口
* [main.pdf](main.pdf)初始文档，让你知道产生的文档是什么样子的，另外包含一些有帮助的基本信息
* [nkthesis.bib](nkthesis.bib) 参考文献bib文件，可使用Google学术或百度学术直接导出bibtex格式
* [tex/文件夹](tex/) 每一章单独一个文件,主要写作部分

### 其他

* 支持绘图
* 支持语法高亮

## 最后祝各位顺利毕业！
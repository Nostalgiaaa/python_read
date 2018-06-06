# Text



## Text

The `str` class is the most obvious text processing tool available to Python programmers, but there are plenty of other tools in the standard library to make advanced text manipulation simple.

在 Python 程序中最容易被用到处理文本的类是 str 类，但标准库中有许多其他工具可以使高级文本操作变得简单。

Programs may use `string.Template` as a simple way to parameterize strings beyond the features of `str` objects. While not as feature-rich as templates defined by many of the web frameworks or extension modules available from the Python Package Index, `string.Template` is a good middle ground for user-modifiable templates in which dynamic values need to be inserted into otherwise static text.

程序可以使用 string.Template 这种更简单的方式来对 str 对象特征之外的字符串进行参数化。  
虽然不像许多Web框架或扩展模块定义的模板那样功能丰富\(例如jinja2\)，但是 string.Template 是用户可修改的模板\(动态值需要插入到静态文本中\)的一个很好的中间层。

The [`textwrap`](https://pymotw.com/3/textwrap/index.html#module-textwrap) module includes tools for formatting text from paragraphs by limiting the width of output, adding indentation, and inserting line breaks to wrap lines consistently.

textwrap 模块是一个可以通过限制输出宽度，添加缩进和插入换行符这些功能来一致地对段落中的文本进行格式设置的工具。

The standard library includes two modules for comparing text values that go beyond the built-in equality and sort comparison supported by string objects. [`re`](https://pymotw.com/3/re/index.html#module-re) provides a complete regular expression library, implemented in C for speed. Regular expressions are well suited for finding substrings within a larger data set, comparing strings against a pattern more complex than another fixed string, and mild parsing.

标准库包含两个模块，用来比较超出字符串对象支持的内置等式和排序比较的文本值。re 是一个有着C语言执行速度的完整的正则表达式库。正则表达式非常适合以下几个场景:

* 特别大的数据集中查找子字符串。
* 将字符串用更复杂的模式与另一个固定字符串进行比较。\(此处翻译不太通。。\)
* 轻松解析字符串

[`difflib`](https://pymotw.com/3/difflib/index.html#module-difflib), in contrast, computes the actual differences between sequences of text in terms of the parts added, removed, or changed. The output of the comparison functions in [`difflib`](https://pymotw.com/3/difflib/index.html#module-difflib) can be used to provide more detailed feedback to the user about where changes occur in two inputs, how a document has changed over time, and so on.

跟re相反，difflib 根据不同\(增删改\)的部分计算文本序列之间的实际差异。 difflib 中比较函数的输出可用于向用户提供更详细的反馈，以提供有关两个输入发生变化的位置，文档如何随时间变化等等。

* [string — Text Constants and Templates](https://pymotw.com/3/string/index.html)
* [textwrap — Formatting Text Paragraphs](https://pymotw.com/3/textwrap/index.html)
* [re — Regular Expressions](https://pymotw.com/3/re/index.html)
* [difflib — Compare Sequences](https://pymotw.com/3/difflib/index.html)


# CompilingPrinciple

1. lex 文件夹

> 此文件夹有 3 个 *Java类* ，这三个类的终极目标是实现:自动生成任意语言的 **词法分析器** 。就像 **lex/flex**。水平有限只粗糙实现了核心算法以作练习。

- `Thompson.java` 实现：**Re(正则表达式)** --> **NFA**，使用的是 `Thompson算法`；
- `SubsetConstruction.java` 实现： **NFA** --> **DFA**，使用的是 `子集构造算法`；
- `Hopcroft.java` 实现：**优化DFA**，使用的是 `Hopcroft算法`；
- 最后的一个 *表驱动算法* ，由于对于输入、输出没有确定，没有写完，故没有粘贴。

2. flexTool/TinyC 文件夹

> 此文件夹记录了使用 `flex` 工具。用此，实现了对 **TinyC** 语言的词法分析，这种语言是 **C语言** 的一个子集。

- `lexTinyC.l`    **flex文件**
- `token.h`       **上述包含的头文件**
- `lex.yy.c`      **flex产生的文件，注意 yylex() 函数**
- `lexTinyC`      **编译上述文件生成的目标程序**
- `tinyc.c`       **测试代码**
- `result.txt`    **测试结果**
# Chapter 2 开始学习C++

## 目录
* [2.1.6.1: endl](#endl)
* [2.1.7: 原始字符串](#原始字符串)
* [2.4.3.1: 函数嵌套定义](#函数嵌套定义)
* [编程练习](problem/)


### endl

endl 是一个特殊的 C++ 符号，表示一个重要的概念：重起一行。和 cout 一样， endl 是在头文件 iostream 中定义的，且位于名称空间 std 中。

endl 与 '\n' 不同的地方在于： endl 可以保证在程序运行前刷新输出，即保证之前的输出显示在屏幕上。我以前遇到过这样的问题：在debug的时候，输出中间结果的代码一直不执行，最后发现就是因为我没有使用 endl 或者 ends 这样的方式来刷新输出。


### 原始字符串

C++11新特性，原始字符串内部可包含回车等符号，内部不进行转义。

使用方法：R"(字符串)"。

原始字符串可以通过修改开头来使内部可以包含 ')'。 [2-1-7.cpp](2-1-7.cpp)


### 函数嵌套定义

C/C++ 不允许将函数定义嵌套在另一个函数定义中

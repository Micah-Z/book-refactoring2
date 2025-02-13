# Table of contents

* [简介](README.md)
* [序言](docs/README.md)
* [第 1 章 重构，第一个示例](docs/ch1.md)
  * [1.1 起点](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#11-%E8%B5%B7%E7%82%B9)
  * [1.2 对此起始程序的评价](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#12-%E5%AF%B9%E6%AD%A4%E8%B5%B7%E5%A7%8B%E7%A8%8B%E5%BA%8F%E7%9A%84%E8%AF%84%E4%BB%B7)
  * [1.3 重构的第一步](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#13-%E9%87%8D%E6%9E%84%E7%9A%84%E7%AC%AC%E4%B8%80%E6%AD%A5)
  * [1.4 分解 statement 函数](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#14-%E5%88%86%E8%A7%A3-statement-%E5%87%BD%E6%95%B0)
  * [1.5 进展：大量嵌套函数](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#15-%E8%BF%9B%E5%B1%95%EF%BC%9A%E5%A4%A7%E9%87%8F%E5%B5%8C%E5%A5%97%E5%87%BD%E6%95%B0)
  * [1.6 拆分计算阶段与格式化阶段](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#16-%E6%8B%86%E5%88%86%E8%AE%A1%E7%AE%97%E9%98%B6%E6%AE%B5%E4%B8%8E%E6%A0%BC%E5%BC%8F%E5%8C%96%E9%98%B6%E6%AE%B5)
  * [1.7 进展：分离到两个文件（和两个阶段）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#17-%E8%BF%9B%E5%B1%95%EF%BC%9A%E5%88%86%E7%A6%BB%E5%88%B0%E4%B8%A4%E4%B8%AA%E6%96%87%E4%BB%B6%EF%BC%88%E5%92%8C%E4%B8%A4%E4%B8%AA%E9%98%B6%E6%AE%B5%EF%BC%89)
  * [1.8 按类型重组计算过程](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#18-%E6%8C%89%E7%B1%BB%E5%9E%8B%E9%87%8D%E7%BB%84%E8%AE%A1%E7%AE%97%E8%BF%87%E7%A8%8B)
  * [1.9 进展：使用多态计算器来提供数据](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#19-%E8%BF%9B%E5%B1%95%EF%BC%9A%E4%BD%BF%E7%94%A8%E5%A4%9A%E6%80%81%E8%AE%A1%E7%AE%97%E5%99%A8%E6%9D%A5%E6%8F%90%E4%BE%9B%E6%95%B0%E6%8D%AE)
  * [1.10 结语](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch1#110-%E7%BB%93%E8%AF%AD)
* [第 2 章 重构的原则](docs/ch2.md)
  * [2.1 何谓重构](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#21-%E4%BD%95%E8%B0%93%E9%87%8D%E6%9E%84)
  * [2.2 两顶帽子](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#22-%E4%B8%A4%E9%A1%B6%E5%B8%BD%E5%AD%90)
  * [2.3 为何重构](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#23-%E4%B8%BA%E4%BD%95%E9%87%8D%E6%9E%84)
  * [2.4 何时重构](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#24-%E4%BD%95%E6%97%B6%E9%87%8D%E6%9E%84)
  * [2.5 重构的挑战](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#25-%E9%87%8D%E6%9E%84%E7%9A%84%E6%8C%91%E6%88%98)
  * [2.6 重构、架构和 YAGNI](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#26-%E9%87%8D%E6%9E%84%E3%80%81%E6%9E%B6%E6%9E%84%E5%92%8C-yagni)
  * [2.7 重构与软件开发过程](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#27-%E9%87%8D%E6%9E%84%E4%B8%8E%E8%BD%AF%E4%BB%B6%E5%BC%80%E5%8F%91%E8%BF%87%E7%A8%8B)
  * [2.8 重构与性能](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#28-%E9%87%8D%E6%9E%84%E4%B8%8E%E6%80%A7%E8%83%BD)
  * [2.9 重构起源何处](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#29-%E9%87%8D%E6%9E%84%E8%B5%B7%E6%BA%90%E4%BD%95%E5%A4%84)
  * [2.10 自动化重构](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#210-%E8%87%AA%E5%8A%A8%E5%8C%96%E9%87%8D%E6%9E%84)
  * [2.11 延展阅读](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch2#211-%E5%BB%B6%E5%B1%95%E9%98%85%E8%AF%BB)
* [第 3 章 代码的坏味道](docs/ch3.md)
  * [3.1 神秘命名（Mysterious Name）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#31-%E7%A5%9E%E7%A7%98%E5%91%BD%E5%90%8D%EF%BC%88mysterious-name%EF%BC%89)
  * [3.2 重复代码（Duplicated Code）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#32-%E9%87%8D%E5%A4%8D%E4%BB%A3%E7%A0%81%EF%BC%88duplicated-code%EF%BC%89)
  * [3.3 过长函数（Long Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#33-%E8%BF%87%E9%95%BF%E5%87%BD%E6%95%B0%EF%BC%88long-function%EF%BC%89)
  * [3.4 过长参数列表（Long Parameter List）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#34-%E8%BF%87%E9%95%BF%E5%8F%82%E6%95%B0%E5%88%97%E8%A1%A8%EF%BC%88long-parameter-list%EF%BC%89)
  * [3.5 全局数据（Global Data）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#35-%E5%85%A8%E5%B1%80%E6%95%B0%E6%8D%AE%EF%BC%88global-data%EF%BC%89)
  * [3.6 可变数据（Mutable Data）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#36-%E5%8F%AF%E5%8F%98%E6%95%B0%E6%8D%AE%EF%BC%88mutable-data%EF%BC%89)
  * [3.7 发散式变化（Divergent Change）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#37-%E5%8F%91%E6%95%A3%E5%BC%8F%E5%8F%98%E5%8C%96%EF%BC%88divergent-change%EF%BC%89)
  * [3.8 霰弹式修改（Shotgun Surgery）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#38-%E9%9C%B0%E5%BC%B9%E5%BC%8F%E4%BF%AE%E6%94%B9%EF%BC%88shotgun-surgery%EF%BC%89)
  * [3.9 依恋情结（Feature Envy）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#39-%E4%BE%9D%E6%81%8B%E6%83%85%E7%BB%93%EF%BC%88feature-envy%EF%BC%89)
  * [3.10 数据泥团（Data Clumps）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#310-%E6%95%B0%E6%8D%AE%E6%B3%A5%E5%9B%A2%EF%BC%88data-clumps%EF%BC%89)
  * [3.11 基本类型偏执（Primitive Obsession）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#311-%E5%9F%BA%E6%9C%AC%E7%B1%BB%E5%9E%8B%E5%81%8F%E6%89%A7%EF%BC%88primitive-obsession%EF%BC%89)
  * [3.12 重复的 switch （Repeated Switches）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#312-%E9%87%8D%E5%A4%8D%E7%9A%84-switch-%EF%BC%88repeated-switches%EF%BC%89)
  * [3.13 循环语句（Loops）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#313-%E5%BE%AA%E7%8E%AF%E8%AF%AD%E5%8F%A5%EF%BC%88loops%EF%BC%89)
  * [3.14 冗赘的元素（Lazy Element）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#314-%E5%86%97%E8%B5%98%E7%9A%84%E5%85%83%E7%B4%A0%EF%BC%88lazy-element%EF%BC%89)
  * [3.15 夸夸其谈通用性（Speculative Generality）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#315-%E5%A4%B8%E5%A4%B8%E5%85%B6%E8%B0%88%E9%80%9A%E7%94%A8%E6%80%A7%EF%BC%88speculative-generality%EF%BC%89)
  * [3.16 临时字段（Temporary Field）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#316-%E4%B8%B4%E6%97%B6%E5%AD%97%E6%AE%B5%EF%BC%88temporary-field%EF%BC%89)
  * [3.17 过长的消息链（Message Chains）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#317-%E8%BF%87%E9%95%BF%E7%9A%84%E6%B6%88%E6%81%AF%E9%93%BE%EF%BC%88message-chains%EF%BC%89)
  * [3.18 中间人（Middle Man）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#318-%E4%B8%AD%E9%97%B4%E4%BA%BA%EF%BC%88middle-man%EF%BC%89)
  * [3.19 内幕交易（Insider Trading）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#319-%E5%86%85%E5%B9%95%E4%BA%A4%E6%98%93%EF%BC%88insider-trading%EF%BC%89)
  * [3.20 过大的类（Large Class）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#320-%E8%BF%87%E5%A4%A7%E7%9A%84%E7%B1%BB%EF%BC%88large-class%EF%BC%89)
  * [3.21 异曲同工的类（Alternative Classes with Different Interfaces）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#321-%E5%BC%82%E6%9B%B2%E5%90%8C%E5%B7%A5%E7%9A%84%E7%B1%BB%EF%BC%88alternative-classes-with-different-interfaces%EF%BC%89)
  * [3.22 纯数据类（Data Class）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#322-%E7%BA%AF%E6%95%B0%E6%8D%AE%E7%B1%BB%EF%BC%88data-class%EF%BC%89)
  * [3.23 被拒绝的遗赠（Refused Bequest）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#323-%E8%A2%AB%E6%8B%92%E7%BB%9D%E7%9A%84%E9%81%97%E8%B5%A0%EF%BC%88refused-bequest%EF%BC%89)
  * [3.24 注释（Comments）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch3#324-%E6%B3%A8%E9%87%8A%EF%BC%88comments%EF%BC%89)
* [第 4 章 构筑测试体系](docs/ch4.md)
  * [4.1 自测试代码的价值](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#41-%E8%87%AA%E6%B5%8B%E8%AF%95%E4%BB%A3%E7%A0%81%E7%9A%84%E4%BB%B7%E5%80%BC)
  * [4.2 待测试的示例代码](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#42-%E5%BE%85%E6%B5%8B%E8%AF%95%E7%9A%84%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81)
  * [4.3 第一个测试](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#43-%E7%AC%AC%E4%B8%80%E4%B8%AA%E6%B5%8B%E8%AF%95)
  * [4.4 再添加一个测试](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#44-%E5%86%8D%E6%B7%BB%E5%8A%A0%E4%B8%80%E4%B8%AA%E6%B5%8B%E8%AF%95)
  * [4.5 修改测试夹具](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#45-%E4%BF%AE%E6%94%B9%E6%B5%8B%E8%AF%95%E5%A4%B9%E5%85%B7)
  * [4.6 探测边界条件](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#46-%E6%8E%A2%E6%B5%8B%E8%BE%B9%E7%95%8C%E6%9D%A1%E4%BB%B6)
  * [4.7 测试远不止如此](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch4#47-%E6%B5%8B%E8%AF%95%E8%BF%9C%E4%B8%8D%E6%AD%A2%E5%A6%82%E6%AD%A4)
* [第 5 章 介绍重构名录](docs/ch5.md)
  * [5.1 重构的记录格式](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch5#51-%E9%87%8D%E6%9E%84%E7%9A%84%E8%AE%B0%E5%BD%95%E6%A0%BC%E5%BC%8F)
  * [5.2 挑选重构的依据](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch5#52-%E6%8C%91%E9%80%89%E9%87%8D%E6%9E%84%E7%9A%84%E4%BE%9D%E6%8D%AE)
* [第 6 章 第一组重构](docs/ch6.md)
  * [6.1 提炼函数（Extract Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#61-%E6%8F%90%E7%82%BC%E5%87%BD%E6%95%B0%EF%BC%88extract-function%EF%BC%89)
  * [6.2 内联函数（Inline Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#62-%E5%86%85%E8%81%94%E5%87%BD%E6%95%B0%EF%BC%88inline-function%EF%BC%89)
  * [6.3 提炼变量（Extract Variable）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#63-%E6%8F%90%E7%82%BC%E5%8F%98%E9%87%8F%EF%BC%88extract-variable%EF%BC%89)
  * [6.4 内联变量（Inline Variable）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#64-%E5%86%85%E8%81%94%E5%8F%98%E9%87%8F%EF%BC%88inline-variable%EF%BC%89)
  * [6.5 改变函数声明（Change Function Declaration）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#65-%E6%94%B9%E5%8F%98%E5%87%BD%E6%95%B0%E5%A3%B0%E6%98%8E%EF%BC%88change-function-declaration%EF%BC%89)
  * [6.6 封装变量（Encapsulate Variable）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#66-%E5%B0%81%E8%A3%85%E5%8F%98%E9%87%8F%EF%BC%88encapsulate-variable%EF%BC%89)
  * [6.7 变量改名（Rename Variable）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#67-%E5%8F%98%E9%87%8F%E6%94%B9%E5%90%8D%EF%BC%88rename-variable%EF%BC%89)
  * [6.8 引入参数对象（Introduce Parameter Object）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#68-%E5%BC%95%E5%85%A5%E5%8F%82%E6%95%B0%E5%AF%B9%E8%B1%A1%EF%BC%88introduce-parameter-object%EF%BC%89)
  * [6.9 函数组合成类（Combine Functions into Class）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#69-%E5%87%BD%E6%95%B0%E7%BB%84%E5%90%88%E6%88%90%E7%B1%BB%EF%BC%88combine-functions-into-class%EF%BC%89)
  * [6.10 函数组合成变换（Combine Functions into Transform）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#610-%E5%87%BD%E6%95%B0%E7%BB%84%E5%90%88%E6%88%90%E5%8F%98%E6%8D%A2%EF%BC%88combine-functions-into-transform%EF%BC%89)
  * [6.11 拆分阶段（Split Phase）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch6#611-%E6%8B%86%E5%88%86%E9%98%B6%E6%AE%B5%EF%BC%88split-phase%EF%BC%89)
* [第 7 章 封装](docs/ch7.md)
  * [7.1 封装记录（Encapsulate Record）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#71-%E5%B0%81%E8%A3%85%E8%AE%B0%E5%BD%95%EF%BC%88encapsulate-record%EF%BC%89)
  * [7.2 封装集合（Encapsulate Collection）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#72-%E5%B0%81%E8%A3%85%E9%9B%86%E5%90%88%EF%BC%88encapsulate-collection%EF%BC%89)
  * [7.3 以对象取代基本类型（Replace Primitive with Object）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#73-%E4%BB%A5%E5%AF%B9%E8%B1%A1%E5%8F%96%E4%BB%A3%E5%9F%BA%E6%9C%AC%E7%B1%BB%E5%9E%8B%EF%BC%88replace-primitive-with-object%EF%BC%89)
  * [7.4 以查询取代临时变量（Replace Temp with Query）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#74-%E4%BB%A5%E6%9F%A5%E8%AF%A2%E5%8F%96%E4%BB%A3%E4%B8%B4%E6%97%B6%E5%8F%98%E9%87%8F%EF%BC%88replace-temp-with-query%EF%BC%89)
  * [7.5 提炼类（Extract Class）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#75-%E6%8F%90%E7%82%BC%E7%B1%BB%EF%BC%88extract-class%EF%BC%89)
  * [7.6 内联类（Inline Class）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#76-%E5%86%85%E8%81%94%E7%B1%BB%EF%BC%88inline-class%EF%BC%89)
  * [7.7 隐藏委托关系（Hide Delegate）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#77-%E9%9A%90%E8%97%8F%E5%A7%94%E6%89%98%E5%85%B3%E7%B3%BB%EF%BC%88hide-delegate%EF%BC%89)
  * [7.8 移除中间人（Remove Middle Man）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#78-%E7%A7%BB%E9%99%A4%E4%B8%AD%E9%97%B4%E4%BA%BA%EF%BC%88remove-middle-man%EF%BC%89)
  * [7.9 替换算法（Substitute Algorithm）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch7#79-%E6%9B%BF%E6%8D%A2%E7%AE%97%E6%B3%95%EF%BC%88substitute-algorithm%EF%BC%89)
* [第 8 章 搬移特性](docs/ch8.md)
  * [8.1 搬移函数（Move Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#81-%E6%90%AC%E7%A7%BB%E5%87%BD%E6%95%B0%EF%BC%88move-function%EF%BC%89)
  * [8.2 搬移字段（Move Field）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#82-%E6%90%AC%E7%A7%BB%E5%AD%97%E6%AE%B5%EF%BC%88move-field%EF%BC%89)
  * [8.3 搬移语句到函数（Move Statements into Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#83-%E6%90%AC%E7%A7%BB%E8%AF%AD%E5%8F%A5%E5%88%B0%E5%87%BD%E6%95%B0%EF%BC%88move-statements-into-function%EF%BC%89)
  * [8.4 搬移语句到调用者（Move Statements to Callers）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#84-%E6%90%AC%E7%A7%BB%E8%AF%AD%E5%8F%A5%E5%88%B0%E8%B0%83%E7%94%A8%E8%80%85%EF%BC%88move-statements-to-callers%EF%BC%89)
  * [8.5 以函数调用取代内联代码（Replace Inline Code with Function Call）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#85-%E4%BB%A5%E5%87%BD%E6%95%B0%E8%B0%83%E7%94%A8%E5%8F%96%E4%BB%A3%E5%86%85%E8%81%94%E4%BB%A3%E7%A0%81%EF%BC%88replace-inline-code-with-function-call%EF%BC%89)
  * [8.6 移动语句（Slide Statements）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#86-%E7%A7%BB%E5%8A%A8%E8%AF%AD%E5%8F%A5%EF%BC%88slide-statements%EF%BC%89)
  * [8.7 拆分循环（Split Loop）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#87-%E6%8B%86%E5%88%86%E5%BE%AA%E7%8E%AF%EF%BC%88split-loop%EF%BC%89)
  * [8.8 以管道取代循环（Replace Loop with Pipeline）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#88-%E4%BB%A5%E7%AE%A1%E9%81%93%E5%8F%96%E4%BB%A3%E5%BE%AA%E7%8E%AF%EF%BC%88replace-loop-with-pipeline%EF%BC%89)
  * [8.9 移除死代码（Remove Dead Code）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch8#89-%E7%A7%BB%E9%99%A4%E6%AD%BB%E4%BB%A3%E7%A0%81%EF%BC%88remove-dead-code%EF%BC%89)
* [第 9 章 重新组织数据](docs/ch9.md)
  * [9.1 拆分变量（Split Variable）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch9#91-%E6%8B%86%E5%88%86%E5%8F%98%E9%87%8F%EF%BC%88split-variable%EF%BC%89)
  * [9.2 字段改名（Rename Field）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch9#92-%E5%AD%97%E6%AE%B5%E6%94%B9%E5%90%8D%EF%BC%88rename-field%EF%BC%89)
  * [9.3 以查询取代派生变量（Replace Derived Variable with Query）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch9#93-%E4%BB%A5%E6%9F%A5%E8%AF%A2%E5%8F%96%E4%BB%A3%E6%B4%BE%E7%94%9F%E5%8F%98%E9%87%8F%EF%BC%88replace-derived-variable-with-query%EF%BC%89)
  * [9.4 将引用对象改为值对象（Change Reference to Value）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch9#94-%E5%B0%86%E5%BC%95%E7%94%A8%E5%AF%B9%E8%B1%A1%E6%94%B9%E4%B8%BA%E5%80%BC%E5%AF%B9%E8%B1%A1%EF%BC%88change-reference-to-value%EF%BC%89)
  * [9.5 将值对象改为引用对象（Change Value to Reference）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch9#95-%E5%B0%86%E5%80%BC%E5%AF%B9%E8%B1%A1%E6%94%B9%E4%B8%BA%E5%BC%95%E7%94%A8%E5%AF%B9%E8%B1%A1%EF%BC%88change-value-to-reference%EF%BC%89)
* [第 10 章 简化条件逻辑](docs/ch10.md)
  * [10.1 分解条件表达式（Decompose Conditional）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#101-%E5%88%86%E8%A7%A3%E6%9D%A1%E4%BB%B6%E8%A1%A8%E8%BE%BE%E5%BC%8F%EF%BC%88decompose-conditional%EF%BC%89)
  * [10.2 合并条件表达式（Consolidate Conditional Expression）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#102-%E5%90%88%E5%B9%B6%E6%9D%A1%E4%BB%B6%E8%A1%A8%E8%BE%BE%E5%BC%8F%EF%BC%88consolidate-conditional-expression%EF%BC%89)
  * [10.3 以卫语句取代嵌套条件表达式（Replace Nested Conditional with Guard Clauses）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#103-%E4%BB%A5%E5%8D%AB%E8%AF%AD%E5%8F%A5%E5%8F%96%E4%BB%A3%E5%B5%8C%E5%A5%97%E6%9D%A1%E4%BB%B6%E8%A1%A8%E8%BE%BE%E5%BC%8F%EF%BC%88replace-nested-conditional-with-guard-clauses%EF%BC%89)
  * [10.4 以多态取代条件表达式（Replace Conditional with Polymorphism）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#104-%E4%BB%A5%E5%A4%9A%E6%80%81%E5%8F%96%E4%BB%A3%E6%9D%A1%E4%BB%B6%E8%A1%A8%E8%BE%BE%E5%BC%8F%EF%BC%88replace-conditional-with-polymorphism%EF%BC%89)
  * [10.5 引入特例（Introduce Special Case）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#105-%E5%BC%95%E5%85%A5%E7%89%B9%E4%BE%8B%EF%BC%88introduce-special-case%EF%BC%89)
  * [10.6 引入断言（Introduce Assertion）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch10#106-%E5%BC%95%E5%85%A5%E6%96%AD%E8%A8%80%EF%BC%88introduce-assertion%EF%BC%89)
* [第 11 章 重构 API](docs/ch11.md)
  * [11.1 将查询函数和修改函数分离（Separate Query from Modifier）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#111-%E5%B0%86%E6%9F%A5%E8%AF%A2%E5%87%BD%E6%95%B0%E5%92%8C%E4%BF%AE%E6%94%B9%E5%87%BD%E6%95%B0%E5%88%86%E7%A6%BB%EF%BC%88separate-query-from-modifier%EF%BC%89)
  * [11.2 函数参数化（Parameterize Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#112-%E5%87%BD%E6%95%B0%E5%8F%82%E6%95%B0%E5%8C%96%EF%BC%88parameterize-function%EF%BC%89)
  * [11.3 移除标记参数（Remove Flag Argument）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#113-%E7%A7%BB%E9%99%A4%E6%A0%87%E8%AE%B0%E5%8F%82%E6%95%B0%EF%BC%88remove-flag-argument%EF%BC%89)
  * [11.4 保持对象完整（Preserve Whole Object）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#114-%E4%BF%9D%E6%8C%81%E5%AF%B9%E8%B1%A1%E5%AE%8C%E6%95%B4%EF%BC%88preserve-whole-object%EF%BC%89)
  * [11.5 以查询取代参数（Replace Parameter with Query）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#115-%E4%BB%A5%E6%9F%A5%E8%AF%A2%E5%8F%96%E4%BB%A3%E5%8F%82%E6%95%B0%EF%BC%88replace-parameter-with-query%EF%BC%89)
  * [11.6 以参数取代查询（Replace Query with Parameter）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#116-%E4%BB%A5%E5%8F%82%E6%95%B0%E5%8F%96%E4%BB%A3%E6%9F%A5%E8%AF%A2%EF%BC%88replace-query-with-parameter%EF%BC%89)
  * [11.7 移除设值函数（Remove Setting Method）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#117-%E7%A7%BB%E9%99%A4%E8%AE%BE%E5%80%BC%E5%87%BD%E6%95%B0%EF%BC%88remove-setting-method%EF%BC%89)
  * [11.8 以工厂函数取代构造函数（Replace Constructor with Factory Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#118-%E4%BB%A5%E5%B7%A5%E5%8E%82%E5%87%BD%E6%95%B0%E5%8F%96%E4%BB%A3%E6%9E%84%E9%80%A0%E5%87%BD%E6%95%B0%EF%BC%88replace-constructor-with-factory-function%EF%BC%89)
  * [11.9 以命令取代函数（Replace Function with Command）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#119-%E4%BB%A5%E5%91%BD%E4%BB%A4%E5%8F%96%E4%BB%A3%E5%87%BD%E6%95%B0%EF%BC%88replace-function-with-command%EF%BC%89)
  * [11.10 以函数取代命令（Replace Command with Function）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch11#1110-%E4%BB%A5%E5%87%BD%E6%95%B0%E5%8F%96%E4%BB%A3%E5%91%BD%E4%BB%A4%EF%BC%88replace-command-with-function%EF%BC%89)
* [第 12 章 处理继承关系](docs/ch12.md)
  * [12.1 函数上移（Pull Up Method）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#121-%E5%87%BD%E6%95%B0%E4%B8%8A%E7%A7%BB%EF%BC%88pull-up-method%EF%BC%89)
  * [12.2 字段上移（Pull Up Field）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#122-%E5%AD%97%E6%AE%B5%E4%B8%8A%E7%A7%BB%EF%BC%88pull-up-field%EF%BC%89)
  * [12.3 构造函数本体上移（Pull Up Constructor Body）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#123-%E6%9E%84%E9%80%A0%E5%87%BD%E6%95%B0%E6%9C%AC%E4%BD%93%E4%B8%8A%E7%A7%BB%EF%BC%88pull-up-constructor-body%EF%BC%89)
  * [12.4 函数下移（Push Down Method）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#124-%E5%87%BD%E6%95%B0%E4%B8%8B%E7%A7%BB%EF%BC%88push-down-method%EF%BC%89)
  * [12.5 字段下移（Push Down Field）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#125-%E5%AD%97%E6%AE%B5%E4%B8%8B%E7%A7%BB%EF%BC%88push-down-field%EF%BC%89)
  * [12.6 以子类取代类型码（Replace Type Code with Subclasses）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#126-%E4%BB%A5%E5%AD%90%E7%B1%BB%E5%8F%96%E4%BB%A3%E7%B1%BB%E5%9E%8B%E7%A0%81%EF%BC%88replace-type-code-with-subclasses%EF%BC%89)
  * [12.7 移除子类（Remove Subclass）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#127-%E7%A7%BB%E9%99%A4%E5%AD%90%E7%B1%BB%EF%BC%88remove-subclass%EF%BC%89)
  * [12.8 提炼超类（Extract Superclass）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#128-%E6%8F%90%E7%82%BC%E8%B6%85%E7%B1%BB%EF%BC%88extract-superclass%EF%BC%89)
  * [12.9 折叠继承体系（Collapse Hierarchy）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#129-%E6%8A%98%E5%8F%A0%E7%BB%A7%E6%89%BF%E4%BD%93%E7%B3%BB%EF%BC%88collapse-hierarchy%EF%BC%89)
  * [12.10 以委托取代子类（Replace Subclass with Delegate）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#1210-%E4%BB%A5%E5%A7%94%E6%89%98%E5%8F%96%E4%BB%A3%E5%AD%90%E7%B1%BB%EF%BC%88replace-subclass-with-delegate%EF%BC%89)
  * [12.11 以委托取代超类（Replace Superclass with Delegate）](https://app.gitbook.com/s/JtQbu7QFjvEwYj0dYZfm/ch12#1211-%E4%BB%A5%E5%A7%94%E6%89%98%E5%8F%96%E4%BB%A3%E8%B6%85%E7%B1%BB%EF%BC%88replace-superclass-with-delegate%EF%BC%89)

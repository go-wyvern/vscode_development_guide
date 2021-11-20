# vscode 插件开发指南

大家都知道 vscode 是微软推出的一个轻量级的代码编辑器，之所以说他是轻量级，是因为vscode 设计的初衷并不是想让他成为一个大而全的代码编辑器，因为再强大的IDE也不能够做到面面俱到，那样只能让IDE变的臃肿。vscode 几乎所有的功能都是可以都过插件实现，用户可以根据自己的需求，按需下载。IDE只提供一个最基本的框子和最基本功能，由插件来丰富和扩展它的功能。

vscode 插件有非常多种，比如主题类的，模板渲染类的，编程语言类的等。本指南主要会围绕编程语言的插件，并通过go语言插件的实现原理，帮助大家上手vscode 插件开发。并希望能有更多的同学参与到 [vscode-goplus](https://github.com/gopcode/vscode-goplus) 的开发中来。

因为vscode本身都是用浏览器实现的，所以其插件不用说肯定也是基于HTML+JS等前端技术实现，熟悉 npm 开发模式的，上手会比较快，所以vscode插件开发难度不大，甚至可以说熟悉了相关API之后很容易。

vscode 官网实际上提供了一个完整的 [Programmatic Language Features](https://code.visualstudio.com/api/language-extensions/programmatic-language-features) 的接口, 但是可能因为英文，并且没有具体的实现案例，导致很多同学在插件开发过程中难以踏出第一步。本指南将结合go语言插件，尽可能详尽的解析各个语言类的feature 是如何实现的。


具体涉及的知识点如下：

* [第1章 package.json详解](chapter1/README.md)
* [第2章 命令、菜单、快捷键](chapter2/README.md)
* [第3章 语法高亮](chapter3/README.md)
* [第4章 代码片段](chapter4/README.md)
* [第5章 语句折叠，括号定义，注释，自动关闭](chapter5/README.md)
* [第6章 悬停提示](chapter6/README.md)
* [第7章 函数和方法的帮助提示](chapter7/README.md)
* [第8章 跳转到定义](chapter8/README.md)
* [第9章 查找引用](chapter9/README.md)
* [第10章 自动补全](chapter10/README.md)
* [第11章 代码格式化](chapter11/README.md)
* [第12章 语言服务器扩展指南](chapter12/README.md)
* [第13章 打包、发布、升级](chapter13/README.md)

## 版权

版权归 Goplus开发者团队所有，未经许可，禁止转载。
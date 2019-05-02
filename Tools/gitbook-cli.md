# 第1节：gitbook-cli

它是基于nodeJS的命令工具，通过执行gitbook的命令，可以将Markdown 和 AsciiDoc 语法格式的文件转换成 HTML、PDF、eBook。

## 安装和使用

1. 全局安装gitbook命令工具`npm install -g gitbook-cli`

2. 创建一个目录并初始化`gitbook init` ,生成两个文件

  - README.md —— 书籍的介绍
  - SUMMARY.md —— 书籍的目录结构，添加内容如下：

  ```markdown
  # 目录
  
  * [前言](README.md)
  * [第一章 工具](Chapter1/README.md)
      * [第1节：gitbook-cli](Chapter1/gitbook-cli.md)
  * [第二章](Chapter2/README.md)
  * [第三章](Chapter3/README.md)
  * [第四章](Chapter4/README.md)
  ```

3. 再次执行 `gitbook init` 命令，可生成SUMMARY.md内容里没有的目录和文件。

4. 执行 `gitbook serve` 来预览这本书籍，最后提示 “Serving book on [http://localhost:4000](http://localhost:4000/)”

5. 执行 `gitbook build` 命令构建HTML，默认将生成的静态网站输出到 _book 目录

6. 安装ebook-convert, https://calibre-ebook.com

7. 执行`gitbook pdf ./ ./doc.pdf`命令构建PDF

8. more `gitbook help`



# 附：Markdown 编辑工具

[ypora 下载](<https://typora.io/>)，一个非常简洁的Markdown 编辑工具，支持预览模式下编写。

第一次打开，请查看 **显示** 菜单，可以切换编辑区域的显示方式、打开左侧文件树等。
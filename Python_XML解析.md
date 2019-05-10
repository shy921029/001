# Python 对 XML 的解析

Python 对XML有三种解析方法：

- SAX
- DOM
- ElementTree

## SAX(simple API for XML)

Python 标准库包含SAX解析器，SAX用事件驱动模型，
通过在解析XML的过程中触发事件并调用用户定义的
回调函数来处理XML文件

### 使用 SAX 解析 XML

利用 SAX 解析 XML 文档牵涉到两个部分：**解析器**和**事件处理器**

<https://docs.python.org/3/library/xml.sax.html>

## DOM(Document Object Model)

将XML数据在内存中解析成一个树，通过对树的操作来操作XML.

DOM 需要将 XML 数据映射到内存中的树，一是比较慢，二是比较耗内存，而 SAX 流式读取 XML 文件，比较快，占用内存少，但需要用户实现回调函数（handler）

<https://docs.python.org/3/library/xml.dom.html>

## ElementTree

ElementTree 就像一个轻量级的 DOM，具有方便友好的 API。代码可用性好，速度快，消耗内存少。

<https://docs.python.org/3/library/xml.etree.elementtree.html>
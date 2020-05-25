# XML(eXtensible Markup Language)

XML被设计用来传输和存储数据，是各种应用程序之间进行数据传输的最常用工具
HTML被设计用来显示数据
XML可以自定义标签

## XML文档示例

```XML
<?xml version="1.0" encoding="UTF-8"?>
<note>
<to>Tom</to>
<from>Jack</from>
<heading>Reminder</heading>
<body>Don't forget this weekend</body>
</note>
```

第一行是XML声明，定义XML版本和所使用的编码，
第二行是描述文档的根元素，
第3-6行是描述根的4个子元素，
最后一行是根元素的结尾，
元素形成了一棵文档树。

## XML语法规则

- 1.XML文档必须有根元素
- 2.声明需放在第一行
- 3.所有元素都必须有一个关闭标签
- 4.标签对大小写敏感
- 5.元素标签必须正确嵌套

```XML
<b><i>xxxx</i></b>
```

- 6.属性值必须加引号, version="1.0"
- 7.特殊字符需实体引用

字符 | 引用 | 含义
:-: | :-: | :-:
< | &lt | less than
> | &gt | greater than
& | &amp | ampersand
' | &apos | apostrophe
" | &quot | quotation mark

- 8.注释语法与HTML很相似

```XML
<!-- This is a comment -->
```

- 9.HTML中会把多个连续空格字符裁剪(合并)为一个，XML中则不会
- 10.XML 以换行符LF存储换行

## XML元素

XML元素指的是从(且包括)开始标签到(且包括)结束标签的部分，
一个元素可以包含：

- 子元素
- 文本
- 属性

XML元素可扩展，XML的优势之一就是可以在不中断应用程序的情况下进行扩展

### 元素命名规则

- 名称可以包含字母、数字及其他字符
- 不能以数字或标点符号开始
- 不能以字母xml(或XML、Xml等)开始
- 不能包含空格
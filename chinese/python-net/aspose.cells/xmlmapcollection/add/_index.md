---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/xmlmapcollection/add/
is_root: false
---
##  add(url) {#str}
通过 xml/xsd 文件的 url/路径添加 [XmlMap](/cells/zh/python-net/aspose.cells/xmlmap)。


### 返回

[XmlMap](/cells/zh/python-net/aspose.cells/xmlmap) 对象索引。


```python
def add(self, url):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| url | str | xml/xsd 文件的 url/路径。|

### 例子

以下代码通过一个 xsd 文件和一个 xml 文件添加两个 XmlMap。

```python
from aspose.cells import Workbook

wb = Workbook()
xmlMapCollection = wb.worksheets.xml_maps
# Add a XmlMap by a xsd file.
xmlMapCollection.add("schema.xsd")
# Add a XmlMap by a xml file.
xmlMapCollection.add("xml.xml")
wb.save("twoXmlMaps.xlsx")

```



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [XmlMap](/cells/zh/python-net/aspose.cells/xmlmap)
* 类 [XmlMapCollection](/cells/zh/python-net/aspose.cells/xmlmapcollection)

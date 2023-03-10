---
title: export_xml方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 140
url: /zh/python-net/aspose.cells/workbook/export_xml/
is_root: false
---
##  export_xml(map_name, path) {#str-str}
导出由指定 XML 映射链接的 XML 数据。



```python
def export_xml(self, map_name, path):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| map_name | str |需要导出的XML映射名称|
| path | str |导出路径|

### 例子

以下代码导出了第一个 XmlMap 链接的数据。

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


##  export_xml(map_name, stream) {#str-io.RawIOBase}
导出 XML 数据。



```python
def export_xml(self, map_name, stream):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| map_name | str |需要导出的XML映射名称|
| stream | io.RawIOBase |导出流|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)

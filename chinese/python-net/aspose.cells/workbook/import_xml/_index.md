---
title: import_xml方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 220
url: /zh/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
将 XML 数据文件导入/更新到工作簿中。



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| url | str | xml 文件的 url/路径。|
| sheet_name | str |目标工作表名称。|
| row | int |目标行|
| col | int |目标列|

### 例子

以下代码将 xml 数据导入到位于 Cell A1 的工作表“工作表 1”中。

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
将 XML 数据文件导入/更新到工作簿中。



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase | xml文件流。|
| sheet_name | str |目标工作表名称。|
| row | int |目标行。|
| col | int |目标列。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)

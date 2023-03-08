---
title: PdfBookmarkEntry类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells.rendering/pdfbookmarkentry/
is_root: false
---
##  PdfBookmarkEntry类
PdfBookmarkEntry 是 pdf 书签中的条目。
如果当前实例的 Text 属性为 null 或 ""，
当前实例将被隐藏，子实例将被插入到当前级别。



PdfBookmarkEntry 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [PdfBookmarkEntry()](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/__init__/#) |构造 PdfBookmarkEntry 的新实例|


### 特性
|属性|描述|
| :- | :- |
| [text](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/text) |书签的标题。|
| [destination](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/destination) |书签链接到的单元格。|
| [destination_name](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/destination_name) |获取或设置目的地名称。|
| [sub_entry](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/sub_entry) |书签的子条目。|
| [is_open](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/is_open) |当此属性为真时，书签条目将展开，否则将折叠。|
| [is_collapse](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry/is_collapse) |当此属性为真时，书签条目将折叠，否则将展开。|



### 例子

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering import PdfBookmarkEntry

workbook = Workbook()
workbook.worksheets.add()
workbook.worksheets.add()
cellInPage1 = workbook.worksheets[0].cells.get("A1")
cellInPage2 = workbook.worksheets[1].cells.get("A1")
cellInPage3 = workbook.worksheets[2].cells.get("A1")
cellInPage1.put_value("page1")
cellInPage2.put_value("page2")
cellInPage3.put_value("page3")
pbeRoot = PdfBookmarkEntry()
pbeRoot.text = "root"
pbeRoot.destination = cellInPage1
pbeRoot.sub_entry = []
pbeRoot.is_open = False
subPbe1 = PdfBookmarkEntry()
subPbe1.text = "section1"
subPbe1.destination = cellInPage2
subPbe2 = PdfBookmarkEntry()
subPbe2.text = "section2"
subPbe2.destination = cellInPage3
pbeRoot.sub_entry.append(subPbe1)
pbeRoot.sub_entry.append(subPbe2)
saveOptions = PdfSaveOptions()
saveOptions.bookmark = pbeRoot
workbook.save("output_bookmark.pdf", saveOptions)

```

### 也可以看看
* 模块 [aspose.cells.rendering](..)

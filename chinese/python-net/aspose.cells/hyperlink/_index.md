---
title: Hyperlink类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 790
url: /zh/python-net/aspose.cells/hyperlink/
is_root: false
---
## Hyperlink类
封装表示超链接的对象。



Hyperlink 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [address](/cells/zh/python-net/aspose.cells/hyperlink/address) |表示超链接的地址。|
| [text_to_display](/cells/zh/python-net/aspose.cells/hyperlink/text_to_display) |表示要为指定超链接显示的文本。|
| [area](/cells/zh/python-net/aspose.cells/hyperlink/area) |获取超链接的范围。|
| [screen_tip](/cells/zh/python-net/aspose.cells/hyperlink/screen_tip) |返回或设置指定超链接的屏幕提示文本。|
| [link_type](/cells/zh/python-net/aspose.cells/hyperlink/link_type) |获取链接类型。|


### 方法
|方法|描述|
| :- | :- |
| [delete()](/cells/zh/python-net/aspose.cells/hyperlink/delete/#) |删除此超链接|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Adding a hyperlink to a URL at "A1" cell
index = worksheet.hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Getting a Hyperlink by index.
hyperlink = worksheet.hyperlinks[index]
# Setting display text of this hyperlink.
hyperlink.text_to_display = "Aspose"
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)

---
title: FontSetting类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 670
url: /zh/python-net/aspose.cells/fontsetting/
is_root: false
---
## FontSetting类
表示单元格文本中的一系列字符。



FontSetting 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/zh/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


### 特性
|属性|描述|
| :- | :- |
| [type](/cells/zh/python-net/aspose.cells/fontsetting/type) |获取文本节点的类型。|
| [start_index](/cells/zh/python-net/aspose.cells/fontsetting/start_index) |获取字符的起始索引。|
| [length](/cells/zh/python-net/aspose.cells/fontsetting/length) |获取字符的长度。|
| [font](/cells/zh/python-net/aspose.cells/fontsetting/font) |返回此对象的字体。|
| [text_options](/cells/zh/python-net/aspose.cells/fontsetting/text_options) |返回文本选项。|


### 方法
|方法|描述|
| :- | :- |
| [set_word_art_style(style)](/cells/zh/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) |设置预设的艺术字样式。|



### 例子

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Visit Aspose!")
# getting charactor
charactor = cell.characters(6, 7)
# Setting the font of selected characters to bold
charactor.font.is_bold = True
# Setting the font color of selected characters to blue
charactor.font.color = Color.blue
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)

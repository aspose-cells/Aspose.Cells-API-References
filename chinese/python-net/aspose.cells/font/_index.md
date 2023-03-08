---
title: Font类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 650
url: /zh/python-net/aspose.cells/font/
is_root: false
---
##  Font类
封装电子表格中使用的字体对象。



Font 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [charset](/cells/zh/python-net/aspose.cells/font/charset) |表示字符集。|
| [is_italic](/cells/zh/python-net/aspose.cells/font/is_italic) |获取或设置一个值，该值指示字体是否为斜体。|
| [is_bold](/cells/zh/python-net/aspose.cells/font/is_bold) |获取或设置一个值，该值指示字体是否为粗体。|
| [caps_type](/cells/zh/python-net/aspose.cells/font/caps_type) |获取和设置文本大写类型。|
| [strike_type](/cells/zh/python-net/aspose.cells/font/strike_type) |获取文本的敲击类型。|
| [is_strikeout](/cells/zh/python-net/aspose.cells/font/is_strikeout) |获取或设置一个值，该值指示字体是否为单删除线。|
| [script_offset](/cells/zh/python-net/aspose.cells/font/script_offset) |获取和设置脚本偏移量，以百分比为单位|
| [is_superscript](/cells/zh/python-net/aspose.cells/font/is_superscript) |获取或设置一个值，该值指示字体是否为超级脚本。|
| [is_subscript](/cells/zh/python-net/aspose.cells/font/is_subscript) |获取或设置一个值，该值指示字体是否为下标。|
| [underline](/cells/zh/python-net/aspose.cells/font/underline) |获取或设置字体下划线类型。|
| [name](/cells/zh/python-net/aspose.cells/font/name) |获取或设置 [Font](/cells/zh/python-net/aspose.cells/font) 的名称。|
| [double_size](/cells/zh/python-net/aspose.cells/font/double_size) |获取和设置字体的双倍大小。|
| [size](/cells/zh/python-net/aspose.cells/font/size) |获取或设置字体的大小。|
| [theme_color](/cells/zh/python-net/aspose.cells/font/theme_color) |获取和设置主题颜色。|
| [color](/cells/zh/python-net/aspose.cells/font/color) |获取或设置字体的颜色。|
| [argb_color](/cells/zh/python-net/aspose.cells/font/argb_color) |使用 32 位 ARGB 值获取和设置颜色。|
| [is_normalize_heights](/cells/zh/python-net/aspose.cells/font/is_normalize_heights) |指示要应用于文本的高度规范化是否运行。|
| [scheme_type](/cells/zh/python-net/aspose.cells/font/scheme_type) |获取和设置字体的方案类型。|


### 方法
|方法|描述|
| :- | :- |
| [equals(font)](/cells/zh/python-net/aspose.cells/font/equals/#Font) |检查两个字体是否相等。|



### 例子

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Font](/cells/zh/python-net/aspose.cells/font)

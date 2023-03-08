---
title: ThemeColor类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1430
url: /zh/python-net/aspose.cells/themecolor/
is_root: false
---
##  ThemeColor类
代表主题颜色。



ThemeColor 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [ThemeColor(type, tint)](/cells/zh/python-net/aspose.cells/themecolor/__init__/#ThemeColorType-float) |  |


### 特性
|属性|描述|
| :- | :- |
| [color_type](/cells/zh/python-net/aspose.cells/themecolor/color_type) |获取和设置主题类型。|
| [tint](/cells/zh/python-net/aspose.cells/themecolor/tint) |获取和设置色调值。|



### 例子

```python
from aspose.cells import BackgroundType, ThemeColor, ThemeColorType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").put_value("Hello World")
style = cells.get("A1").get_style()
# Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.font.theme_color = ThemeColor(ThemeColorType.TEXT2, 0.4)
style.pattern = BackgroundType.SOLID
# Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.foreground_theme_color = ThemeColor(ThemeColorType.BACKGROUND2, -0.75)
cells.get("A1").set_style(style)
# Saving the Excel file
workbook.save("book1.xlsx")

```

### 也可以看看
* 模块 [aspose.cells](..)

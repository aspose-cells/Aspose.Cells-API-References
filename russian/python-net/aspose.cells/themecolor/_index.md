---
title: ThemeColor класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1430
url: /ru/python-net/aspose.cells/themecolor/
is_root: false
---
##  ThemeColor класс
Представляет цвет темы.



Тип ThemeColor предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [ThemeColor(type, tint)](/cells/ru/python-net/aspose.cells/themecolor/__init__/#ThemeColorType-float) |  |


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [color_type](/cells/ru/python-net/aspose.cells/themecolor/color_type) | Получает и задает тип темы.|
| [tint](/cells/ru/python-net/aspose.cells/themecolor/tint) | Получает и задает значение оттенка.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)

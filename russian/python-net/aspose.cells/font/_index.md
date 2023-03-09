---
title: Font класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 650
url: /ru/python-net/aspose.cells/font/
is_root: false
---
##  Font класс
Инкапсулирует объект шрифта, используемый в электронной таблице.



Тип Font предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [charset](/cells/ru/python-net/aspose.cells/font/charset) | Представлять набор символов.|
| [is_italic](/cells/ru/python-net/aspose.cells/font/is_italic) | Получает или задает значение, указывающее, является ли шрифт курсивным.|
| [is_bold](/cells/ru/python-net/aspose.cells/font/is_bold) | Получает или задает значение, указывающее, является ли шрифт полужирным.|
| [caps_type](/cells/ru/python-net/aspose.cells/font/caps_type) | Получает и задает тип прописных букв.|
| [strike_type](/cells/ru/python-net/aspose.cells/font/strike_type) | Получает тип забастовки текста.|
| [is_strikeout](/cells/ru/python-net/aspose.cells/font/is_strikeout) | Получает или задает значение, указывающее, является ли шрифт одинарным перечеркнутым.|
| [script_offset](/cells/ru/python-net/aspose.cells/font/script_offset) | Получает и задает смещение скрипта в процентах|
| [is_superscript](/cells/ru/python-net/aspose.cells/font/is_superscript) | Получает или задает значение, указывающее, является ли шрифт суперсценарным.|
| [is_subscript](/cells/ru/python-net/aspose.cells/font/is_subscript) | Получает или задает значение, указывающее, является ли шрифт подстрочным.|
| [underline](/cells/ru/python-net/aspose.cells/font/underline) | Получает или задает тип подчеркивания шрифта.|
| [name](/cells/ru/python-net/aspose.cells/font/name) | Получает или задает имя [Font](/cells/ru/python-net/aspose.cells/font).|
| [double_size](/cells/ru/python-net/aspose.cells/font/double_size) | Получает и задает двойной размер шрифта.|
| [size](/cells/ru/python-net/aspose.cells/font/size) | Получает или задает размер шрифта.|
| [theme_color](/cells/ru/python-net/aspose.cells/font/theme_color) | Получает и задает цвет темы.|
| [color](/cells/ru/python-net/aspose.cells/font/color) | Получает или задает цвет шрифта.|
| [argb_color](/cells/ru/python-net/aspose.cells/font/argb_color) | Получает и задает цвет с 32-битным значением ARGB.|
| [is_normalize_heights](/cells/ru/python-net/aspose.cells/font/is_normalize_heights) | Указывает, применяется ли нормализация высоты к тексту.|
| [scheme_type](/cells/ru/python-net/aspose.cells/font/scheme_type) | Получает и задает тип схемы шрифта.|


###  Методы
| Метод| Описание|
| :- | :- |
| [equals(font)](/cells/ru/python-net/aspose.cells/font/equals/#Font) | Проверяет, равны ли два шрифта.|



###  Пример

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

###  Смотрите также
* модуль [aspose.cells](..)
* класс [Font](/cells/ru/python-net/aspose.cells/font)

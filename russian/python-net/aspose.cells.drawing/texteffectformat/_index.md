---
title: TextEffectFormat класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 700
url: /ru/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat класс
Содержит свойства и методы, применяемые к объектам WordArt.



Тип TextEffectFormat предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [text](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/text) | Текст в WordArt.|
| [font_name](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/font_name) | Имя шрифта, используемого в WordArt.|
| [font_bold](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Указывает, является ли шрифт полужирным.|
| [font_italic](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Указывает, является ли шрифт курсивом.|
| [rotated_chars](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Если задано значение true, символы в указанном объекте WordArt поворачиваются на 90 градусов относительно ограничивающей формы объекта WordArt.|
| [font_size](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/font_size) | Размер (в пунктах) шрифта, используемого в WordArt.|
| [preset_shape](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Получает и задает предустановленный тип фигуры.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_text_effect(effect)](/cells/ru/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Устанавливает предустановленный текстовый эффект.|



###  Примеры

```python
from aspose.cells import Workbook
from aspose.cells.drawing import MsoPresetTextEffect

# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT1, "Aspose", "Arial", 30, False, False, 0, 0, 0, 0, 100, 200)
textEffectFormat = shapes[0].text_effect
textEffectFormat.set_text_effect(MsoPresetTextEffect.TEXT_EFFECT10)
workbook.save("Book1.xls")

```

###  Смотрите также
* модуль [aspose.cells.drawing](..)

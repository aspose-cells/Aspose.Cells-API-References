---
title: ShapeTextAlignment класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment класс
Представляет настройку выравнивания текста фигуры;



Тип ShapeTextAlignment предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [is_text_wrapped](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Получает и задает тип переноса текста для фигуры, содержащей текст.|
| [rotate_text_with_shape](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Указывает, вращается ли текст с фигурой.|
| [text_vertical_overflow](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Получает и задает тип вертикального переполнения текста для текстового поля.|
| [text_horizontal_overflow](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Получает и задает тип горизонтального переполнения текста для текстового поля.|
| [rotation_angle](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Получает и задает поворот фигуры.|
| [text_vertical_type](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Получает и задает направление текста.|
| [auto_size](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) | Указывает, регулируется ли размер фигуры автоматически в соответствии с ее содержимым.|
| [text_shape_type](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Получает и задает тип преобразования текста.|
| [top_margin_pt](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Возвращает верхнюю границу в баллах|
| [bottom_margin_pt](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Возвращает нижнее поле в баллах|
| [left_margin_pt](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Возвращает левое поле в баллах|
| [right_margin_pt](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Возвращает правое поле в баллах|
| [is_auto_margin](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Указывает, является ли поле текстового фрейма автоматическим.|
| [number_of_columns](/cells/ru/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Получает и задает количество столбцов текста в ограничивающем прямоугольнике.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Смотрите также
* модуль [aspose.cells.drawing.texts](..)

---
title: Style класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1390
url: /ru/python-net/aspose.cells/style/
is_root: false
---
##  Style класс
Представляет стиль отображения документа Excel, например шрифт, цвет, выравнивание, границу и т. д.
Объект Style содержит все атрибуты стиля (шрифт, числовой формат, выравнивание и т. д.) в качестве свойств.



Тип Style предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [Style()](/cells/ru/python-net/aspose.cells/style/__init__/#) | Инициализирует новый экземпляр класса [Style](/cells/ru/python-net/aspose.cells/style).|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [background_theme_color](/cells/ru/python-net/aspose.cells/style/background_theme_color) | Получает и задает цвет фоновой темы.|
| [foreground_theme_color](/cells/ru/python-net/aspose.cells/style/foreground_theme_color) | Получает и задает цвет темы переднего плана.|
| [name](/cells/ru/python-net/aspose.cells/style/name) | Получает или задает имя стиля.|
| [pattern](/cells/ru/python-net/aspose.cells/style/pattern) | Получает или задает тип шаблона фона ячейки.|
| [borders](/cells/ru/python-net/aspose.cells/style/borders) | Получает [BorderCollection](/cells/ru/python-net/aspose.cells/bordercollection) стиля.|
| [background_color](/cells/ru/python-net/aspose.cells/style/background_color) | Получает или задает цвет фона стиля.|
| [background_argb_color](/cells/ru/python-net/aspose.cells/style/background_argb_color) | Получает и задает цвет фона с 32-битным значением ARGB.|
| [foreground_color](/cells/ru/python-net/aspose.cells/style/foreground_color) | Получает или задает цвет переднего плана стиля.|
| [foreground_argb_color](/cells/ru/python-net/aspose.cells/style/foreground_argb_color) | Получает и задает цвет переднего плана с 32-битным значением ARGB.|
| [has_borders](/cells/ru/python-net/aspose.cells/style/has_borders) | Проверяет, установлены ли границы для стиля.|
| [parent_style](/cells/ru/python-net/aspose.cells/style/parent_style) | Получает родительский стиль этого стиля.|
| [indent_level](/cells/ru/python-net/aspose.cells/style/indent_level) | Представляет уровень отступа для ячейки или диапазона. Может быть только целым числом от 0 до 250.|
| [font](/cells/ru/python-net/aspose.cells/style/font) | Получает объект [Style.font](/cells/ru/python-net/aspose.cells/style#font).|
| [rotation_angle](/cells/ru/python-net/aspose.cells/style/rotation_angle) | Представляет угол поворота текста.|
| [horizontal_alignment](/cells/ru/python-net/aspose.cells/style/horizontal_alignment) | Получает или задает тип горизонтального выравнивания текста в ячейке.|
| [vertical_alignment](/cells/ru/python-net/aspose.cells/style/vertical_alignment) | Получает или задает тип вертикального выравнивания текста в ячейке.|
| [is_text_wrapped](/cells/ru/python-net/aspose.cells/style/is_text_wrapped) | Получает или задает значение, указывающее, переносится ли текст в ячейке.|
| [number](/cells/ru/python-net/aspose.cells/style/number) | Получает или задает формат отображения чисел и дат. Шаблоны форматирования различаются для разных регионов.|
| [is_locked](/cells/ru/python-net/aspose.cells/style/is_locked) |Получает или задает значение, указывающее, можно ли изменить ячейку.|
| [custom](/cells/ru/python-net/aspose.cells/style/custom) | Представляет строку пользовательского числового формата этого объекта стиля.<br/>Если пользовательский числовой формат не установлен (например, числовой формат является встроенным), будет возвращено «».|
| [culture_custom](/cells/ru/python-net/aspose.cells/style/culture_custom) | Получает и задает строку шаблона, зависящую от языка и региональных параметров, для числового формата.<br/>Если для этого объекта не задан числовой формат, будет возвращено значение NULL.<br/> Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному числу.|
| [invariant_custom](/cells/ru/python-net/aspose.cells/style/invariant_custom) | Получает независимую от языка и региональных параметров строку шаблона для числового формата.<br/>Если для этого объекта не задан числовой формат, будет возвращено значение NULL.<br/> Если числовой формат является встроенным, будет возвращена строка шаблона, соответствующая встроенному числу.|
| [is_formula_hidden](/cells/ru/python-net/aspose.cells/style/is_formula_hidden) | Указывает, будет ли скрыта формула, если лист защищен.|
| [shrink_to_fit](/cells/ru/python-net/aspose.cells/style/shrink_to_fit) | Представляет, если текст автоматически сжимается, чтобы соответствовать доступной ширине столбца.|
| [text_direction](/cells/ru/python-net/aspose.cells/style/text_direction) | Представляет порядок чтения текста.|
| [is_justify_distributed](/cells/ru/python-net/aspose.cells/style/is_justify_distributed) | Указывает, следует ли использовать выравнивание ячеек по ширине или распределенное выравнивание в последней строке текста.|
| [quote_prefix](/cells/ru/python-net/aspose.cells/style/quote_prefix) | Указывает, начинается ли значение ячейки с одинарной кавычки.|
| [is_gradient](/cells/ru/python-net/aspose.cells/style/is_gradient) | Указывает, является ли затенение ячеек градиентным узором.|
| [is_percent](/cells/ru/python-net/aspose.cells/style/is_percent) | Указывает, является ли числовой формат процентным форматом.|
| [is_date_time](/cells/ru/python-net/aspose.cells/style/is_date_time) | Указывает, является ли числовой формат форматом даты.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_border(border_type, border_style, border_color)](/cells/ru/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Устанавливает границы стиля.|
| [set_border(border_type, border_style, border_color)](/cells/ru/python-net/aspose.cells/style/set_border/#BorderType-CellBorderType-CellsColor) | Устанавливает границы стиля.|
| [set_pattern_color(pattern, color1, color2)](/cells/ru/python-net/aspose.cells/style/set_pattern_color/#BackgroundType-aspose.pydrawing.Color-aspose.pydrawing.Color) | Устанавливает цвет фона.|
| [copy(style)](/cells/ru/python-net/aspose.cells/style/copy/#Style) | Копирует данные из другого объекта стиля|
| [update()](/cells/ru/python-net/aspose.cells/style/update/#) | Примените именованный стиль к стилям ячеек, которые используют этот именованный стиль.<br/>Это работает так же, как нажатие кнопки «ОК» после того, как вы закончили изменять стиль.<br/> Применяется только для именованного стиля.|
| [is_modified(modify_flag)](/cells/ru/python-net/aspose.cells/style/is_modified/#StyleModifyFlag) | Проверяет, были ли изменены указанные свойства стиля.<br/> Используется для стиля ConditionalFormattings, чтобы проверить, следует ли использовать указанные свойства этого стиля при применении ConditionalFormattings к ячейке.|
| [set_custom(custom, builtin_preference)](/cells/ru/python-net/aspose.cells/style/set_custom/#str-bool) | Задает строку пользовательского числового формата ячейки.|
| [set_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/ru/python-net/aspose.cells/style/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-aspose.cells.drawing.GradientStyleType-int) | Задает для указанной заливки двухцветный градиент.|
| [get_two_color_gradient(color1, color2, gradient_style_type, variant)](/cells/ru/python-net/aspose.cells/style/get_two_color_gradient/#aspose.pydrawing.Color&-aspose.pydrawing.Color&-any-any) | Получите настройку двухцветного градиента.|
| [get_two_color_gradient_setting()](/cells/ru/python-net/aspose.cells/style/get_two_color_gradient_setting/#) | Получите настройку двухцветного градиента.|
| [to_json()](/cells/ru/python-net/aspose.cells/style/to_json/#) | Преобразование [Style](/cells/ru/python-net/aspose.cells/style) в данные структуры JSON.|



###  Пример

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

workbook = Workbook()
sheets = workbook.worksheets
cell = sheets[0].cells.get("A1")
style = cell.get_style()
style.font.name = "Times New Roman"
style.font.color = Color.blue
cell.set_style(style)

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [BorderCollection](/cells/ru/python-net/aspose.cells/bordercollection)
* класс [Style](/cells/ru/python-net/aspose.cells/style)

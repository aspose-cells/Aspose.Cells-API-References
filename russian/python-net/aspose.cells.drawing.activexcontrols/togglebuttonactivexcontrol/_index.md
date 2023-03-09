---
title: ToggleButtonActiveXControl класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 130
url: /ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
##  ToggleButtonActiveXControl класс
Представляет элемент управления ActiveX ToggleButton.



**Наследование:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Тип ToggleButtonActiveXControl предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [workbook](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Получает объект [ActiveXControlBase.workbook](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Получает тип элемента управления ActiveX.|
| [width](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) |Получает и задает ширину элемента управления в точках.|
| [height](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Получает и задает высоту элемента управления в пунктах.|
| [mouse_icon](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Получает и задает настраиваемый значок для отображения в качестве указателя мыши для элемента управления.|
| [mouse_pointer](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления.|
| [fore_ole_color](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Получает и задает основной цвет переднего плана.|
| [back_ole_color](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Получает и задает цвет фона.|
| [is_visible](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Указывает, виден ли этот элемент управления.|
| [shadow](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Указывает, показывать ли тень.|
| [linked_cell](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Получает и задает связанную ячейку.|
| [list_fill_range](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Получает и задает диапазон заполнения списка.|
| [data](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Получает и задает двоичные данные элемента управления.|
| [is_enabled](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Указывает, может ли элемент управления получать фокус и реагировать на события, созданные пользователем.|
| [is_locked](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Указывает, заблокированы ли данные в элементе управления для редактирования.|
| [is_transparent](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) | Указывает, является ли элемент управления прозрачным.|
| [is_auto_size](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Указывает, будет ли автоматически изменяться размер элемента управления для отображения всего его содержимого.|
| [ime_mode](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) |Получает и задает режим времени выполнения по умолчанию редактора метода ввода для элемента управления, когда он получает фокус.|
| [font](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Представляет шрифт элемента управления.|
| [text_align](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Представляет, как выровнять текст, используемый элементом управления.|
| [caption](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Получает и задает описательный текст, отображаемый в элементе управления.|
| [picture_position](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Получает и задает расположение изображения элемента управления относительно его заголовка.|
| [special_effect](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Получает и задает специальный эффект элемента управления.|
| [picture](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) | Получает и устанавливает данные изображения.|
| [accelerator](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Получает и задает клавишу быстрого доступа для элемента управления.|
| [value](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) |Указывает, проверен элемент управления или нет.|
| [is_triple_state](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Указывает, как указанный элемент управления будет отображать значения Null.|



###  Примеры

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ToggleButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TOGGLE_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ToggleButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.drawing.activexcontrols](..)
* класс [ActiveXControl](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* класс [ActiveXControlBase](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* класс [ToggleButtonActiveXControl](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)

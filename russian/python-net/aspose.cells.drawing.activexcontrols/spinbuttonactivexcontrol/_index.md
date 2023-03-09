---
title: SpinButtonActiveXControl класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 110
url: /ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---
##  SpinButtonActiveXControl класс
Представляет элемент управления SpinButton.



**Наследование:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



Тип SpinButtonActiveXControl предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [workbook](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Получает объект [ActiveXControlBase.workbook](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook).|
| [type](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Получает тип элемента управления ActiveX.|
| [width](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) |Получает и задает ширину элемента управления в точках.|
| [height](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Получает и задает высоту элемента управления в пунктах.|
| [mouse_icon](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Получает и задает настраиваемый значок для отображения в качестве указателя мыши для элемента управления.|
| [mouse_pointer](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) | Получает и задает тип значка, отображаемого в качестве указателя мыши для элемента управления.|
| [fore_ole_color](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Получает и задает основной цвет переднего плана.|
| [back_ole_color](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Получает и задает цвет фона.|
| [is_visible](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Указывает, виден ли этот элемент управления.|
| [shadow](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Указывает, показывать ли тень.|
| [linked_cell](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Получает и задает связанную ячейку.|
| [list_fill_range](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Получает и задает диапазон заполнения списка.|
| [data](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Получает и задает двоичные данные элемента управления.|
| [is_enabled](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Указывает, может ли элемент управления получать фокус и реагировать на события, созданные пользователем.|
| [is_locked](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Указывает, заблокированы ли данные в элементе управления для редактирования.|
| [is_transparent](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) | Указывает, является ли элемент управления прозрачным.|
| [is_auto_size](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Указывает, будет ли автоматически изменяться размер элемента управления для отображения всего его содержимого.|
| [ime_mode](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) |Получает и задает режим времени выполнения по умолчанию редактора метода ввода для элемента управления, когда он получает фокус.|
| [font](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Представляет шрифт элемента управления.|
| [text_align](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Представляет, как выровнять текст, используемый элементом управления.|
| [min](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Получает и задает минимально допустимое значение.|
| [max](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Получает и задает максимально допустимое значение.|
| [position](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Получает и задает значение.|
| [small_change](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Получает и задает величину, на которую изменяется свойство Position.|
| [orientation](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Получает и задает вертикальную или горизонтальную ориентацию SpinButton или ScrollBar.|



###  Примеры

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, SpinButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(SpinButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.drawing.activexcontrols](..)
* класс [ActiveXControl](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* класс [ActiveXControlBase](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* класс [SpinButtonActiveXControl](/cells/ru/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)

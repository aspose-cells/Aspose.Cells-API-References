---
title: set_style метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells/row/set_style/
is_root: false
---
##  set_style(style) {#Style}
Устанавливает стиль этой строки.



```python
def set_style(self, style):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| style | [Style](/cells/ru/python-net/aspose.cells/style) | стиль, который будет использоваться в качестве стиля по умолчанию для ячеек в этой строке.|
###  Примечания

Этот метод только устанавливает данный стиль в качестве стиля по умолчанию для этой строки,
без изменения настроек стиля для существующих ячеек в этой строке.
Чтобы одновременно обновить настройки стиля существующих ячеек до указанного стиля,
пожалуйста, используйте [Row.apply_style(style, flag)](/cells/ru/python-net/aspose.cells/row/apply_style)


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Row](/cells/ru/python-net/aspose.cells/row)

---
title: get_style метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells/row/get_style/
is_root: false
---
##  get_style() {#}
Получает стиль этой строки.



```python
def get_style(self):
    ...
```


###  Примечания

Изменение возвращенного объекта стиля напрямую не влияет на эту строку или любые ячейки в этой строке.
Вы должны вызвать метод [Row.apply_style(style, flag)](/cells/ru/python-net/aspose.cells/row/apply_style) или [Row.set_style(style)](/cells/ru/python-net/aspose.cells/row/set_style)
чтобы применить изменение к этой строке.

Стиль строки — это стиль, который будет унаследован ячейками в этой строке (теми ячейками, которые не имеют пользовательских настроек стиля,
например, существующие ячейки, стиль которых не был задан явно, или те, которые не были созданы)


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Row](/cells/ru/python-net/aspose.cells/row)

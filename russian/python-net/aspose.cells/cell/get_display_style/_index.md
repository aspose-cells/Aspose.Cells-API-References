---
title: get_display_style метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 110
url: /ru/python-net/aspose.cells/cell/get_display_style/
is_root: false
---
##  get_display_style() {#}
Получает стиль отображения ячейки.
Если на эту ячейку также влияют другие параметры, такие как условное форматирование, объекты списка и т. д.,
тогда стиль отображения может отличаться от cell.GetStyle().



```python
def get_display_style(self):
    ...
```




##  get_display_style(include_merged_borders) {#bool}
Получает стиль отображения ячейки.
Если ячейка имеет условное форматирование, стиль отображения отличается от стиля cell.GetStyle().



```python
def get_display_style(self, include_merged_borders):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| include_merged_borders | bool | Указывает, проверяются ли границы объединенных ячеек.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)

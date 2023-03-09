---
title: CellArea класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 150
url: /ru/python-net/aspose.cells/cellarea/
is_root: false
---
##  CellArea класс
Представляют собой площадь клеток.



Тип CellArea предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [CellArea()](/cells/ru/python-net/aspose.cells/cellarea/__init__/#) | Создает новый экземпляр CellArea|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [start_row](/cells/ru/python-net/aspose.cells/cellarea/start_row) | Получает или задает начальную строку этой области.|
| [end_row](/cells/ru/python-net/aspose.cells/cellarea/end_row) | Получает или задает конечную строку этой области.|
| [start_column](/cells/ru/python-net/aspose.cells/cellarea/start_column) |Получает или задает начальный столбец этой области.|
| [end_column](/cells/ru/python-net/aspose.cells/cellarea/end_column) | Получает или задает конечный столбец этой области.|


###  Методы
| Метод| Описание|
| :- | :- |
| [create_cell_area(start_row, start_column, end_row, end_column)](/cells/ru/python-net/aspose.cells/cellarea/create_cell_area/#int-int-int-int) | Создает область ячеек.|
| [create_cell_area(start_cell_name, end_cell_name)](/cells/ru/python-net/aspose.cells/cellarea/create_cell_area/#str-str) | Создает область ячеек.|
| [compare_to(obj)](/cells/ru/python-net/aspose.cells/cellarea/compare_to/#any) | Сравните два объекта CellArea по их верхнему левому углу.|



###  Примеры

```python
from aspose.cells import CellArea

# Create Cell Area
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0

```

###  Смотрите также
* модуль [aspose.cells](..)

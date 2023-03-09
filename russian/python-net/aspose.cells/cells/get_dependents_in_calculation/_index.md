---
title: get_dependents_in_calculation метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 390
url: /ru/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Получает все ячейки, вычисленный результат которых зависит от определенных ячеек.


###  Возвращает

Перечислитель для перечисления всех иждивенцев (Cell объектов)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| row | int | Индекс строки конкретной ячейки|
| column | int | Индекс столбца конкретной ячейки.|
| recursive | bool | Возвращает ли те иждивенцы, которые не ссылаются на конкретную ячейку напрямую<br/> но ссылка на другие листы этой ячейки.|
###  Примечания

Чтобы использовать этот метод, убедитесь, что в рабочей книге задано истинное значение для
[FormulaSettings.enable_calculation_chain](/cells/ru/python-net/aspose.cells/formulasettings#enable_calculation_chain) и был полностью рассчитан с этой настройкой.
Если в этой ячейке нет ссылки на формулу, будет возвращено значение NULL.
Для получения более подробной информации и примеров, пожалуйста, обращайтесь по телефону [Cell.get_dependents_in_calculation(recursive)](/cells/ru/python-net/aspose.cells/cell/get_dependents_in_calculation).


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)

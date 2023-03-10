---
title: get_dependents_in_calculation метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
Получает все ячейки, результат вычислений которых зависит от этой ячейки.


###  Возвращает

Перечислитель для перечисления всех иждивенцев (Cell объектов)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| recursive | bool | Возвращает ли те иждивенцы, которые не ссылаются на эту ячейку напрямую<br/> но ссылка на другие листы этой ячейки|
###  Примечания

Чтобы использовать этот метод, убедитесь, что в рабочей книге задано истинное значение для
[FormulaSettings.enable_calculation_chain](/cells/ru/python-net/aspose.cells/formulasettings#enable_calculation_chain) и был полностью рассчитан с этой настройкой.
Если в этой ячейке нет ссылки на формулу, будет возвращено значение NULL.
###  Пример

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("B1").get_dependents_in_calculation(False)
print("B1's calculation dependents:")
for c in en:
    print(c.name)
en = cells.get("B2").get_dependents_in_calculation(False)
print("B2's calculation dependents:")
for c in en:
    print(c.name)

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)

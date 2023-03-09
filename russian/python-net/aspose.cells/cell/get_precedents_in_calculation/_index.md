---
title: get_precedents_in_calculation метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 190
url: /ru/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
Получает все прецеденты (ссылки на ячейки в текущей книге), используемые формулой этой ячейки при ее вычислении.


###  Возвращает

Перечислитель для перечисления всех ссылок (Referred Area)


```python
def get_precedents_in_calculation(self):
    ...
```


###  Примечания

Этот метод может работать только в ситуации, когда [FormulaSettings.enable_calculation_chain](/cells/ru/python-net/aspose.cells/formulasettings#enable_calculation_chain)
верно для рабочей книги, и рабочая книга была полностью рассчитана.
Если эта ячейка не является формулой или не ссылается ни на какие другие ячейки, будет возвращено значение NULL.
###  Примеры

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
workbook.settings.formula_settings.enable_calculation_chain = True
workbook.calculate_formula()
en = cells.get("A2").get_precedents_in_calculation()
print("A2's calculation precedents:")
for r in en:
    print(r)

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)

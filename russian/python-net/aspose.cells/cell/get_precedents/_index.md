---
title: get_precedents метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 180
url: /ru/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
Получает все ссылки, встречающиеся в формуле этой ячейки.


###  Возвращает

Коллекция всех ссылок, появляющихся в формуле этой ячейки.


```python
def get_precedents(self):
    ...
```


###  Примечания

* Возвращает значение null, если это не ячейка формулы. Все ссылки, появляющиеся в формуле этой ячейки, будут возвращены независимо от того, используются они или нет при расчете.

Например, хотя ячейка A2 в формуле «=ЕСЛИ(ИСТИНА,A1,A2)» не используется при расчете,
он по-прежнему считается прецедентом формулы. Чтобы получить те ссылки, которые влияют только на расчет, используйте [Cell.get_precedents_in_calculation()](/cells/ru/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Возвращает значение null, если это не ячейка формулы. Все ссылки, появляющиеся в формуле этой ячейки, будут возвращены независимо от того, используются они или нет при расчете.
Например, хотя ячейка A2 в формуле «=ЕСЛИ(ИСТИНА,A1,A2)» не используется при расчете,
он по-прежнему считается прецедентом формулы. Чтобы получить те ссылки, которые влияют только на расчет, используйте [Cell.get_precedents_in_calculation()](/cells/ru/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Возвращает значение null, если это не ячейка формулы. Все ссылки, появляющиеся в формуле этой ячейки, будут возвращены независимо от того, используются они или нет при расчете.
Например, хотя ячейка A2 в формуле «=ЕСЛИ(ИСТИНА,A1,A2)» не используется при расчете,
он по-прежнему считается прецедентом формулы. Чтобы получить те ссылки, которые влияют только на расчет, используйте [Cell.get_precedents_in_calculation()](/cells/ru/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  Примеры

```python
from aspose.cells import CellsHelper, Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1"
areas = cells.get("A1").get_precedents()
for i in range(len(areas)):
    area = areas[i]
    stringBuilder = []
    if area.is_external_link:
        stringBuilder.append("[")
        stringBuilder.append(area.external_file_name)
        stringBuilder.append("]")
    stringBuilder.append(area.sheet_name)
    stringBuilder.append("!")
    stringBuilder.append(CellsHelper.cell_index_to_name(area.start_row, area.start_column))
    if area.is_area:
        stringBuilder.append(":")
        stringBuilder.append(CellsHelper.cell_index_to_name(area.end_row, area.end_column))
    print("".join(stringBuilder))

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cell](/cells/ru/python-net/aspose.cells/cell)

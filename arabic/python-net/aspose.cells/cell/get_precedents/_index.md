---
title: طريقة get_precedents
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 180
url: /ar/python-net/aspose.cells/cell/get_precedents/
is_root: false
---
##  get_precedents() {#}
الحصول على كافة المراجع التي تظهر في صيغة هذه الخلية.


###  عائدات

مجموعة من كافة المراجع التي تظهر في صيغة هذه الخلية.


```python
def get_precedents(self):
    ...
```


###  ملاحظات

* تُرجع القيمة فارغة إذا لم تكن هذه خلية معادلة. سيتم إرجاع جميع المراجع التي تظهر في صيغة هذه الخلية بغض النظر عن الإشارة إليها أو عدم الرجوع إليها أثناء الحساب.

على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا يزال يعتبر بمثابة سوابق للصيغة. للحصول على تلك المراجع التي تؤثر على الحساب فقط ، يرجى استخدام [Cell.get_precedents_in_calculation()](/cells/ar/python-net/aspose.cells/cell/get_precedents_in_calculation).

* تُرجع القيمة فارغة إذا لم تكن هذه خلية معادلة. سيتم إرجاع جميع المراجع التي تظهر في صيغة هذه الخلية بغض النظر عن الإشارة إليها أو عدم الرجوع إليها أثناء الحساب.
على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا يزال يعتبر بمثابة سوابق للصيغة. للحصول على تلك المراجع التي تؤثر على الحساب فقط ، يرجى استخدام [Cell.get_precedents_in_calculation()](/cells/ar/python-net/aspose.cells/cell/get_precedents_in_calculation).

* تُرجع القيمة فارغة إذا لم تكن هذه خلية معادلة. سيتم إرجاع جميع المراجع التي تظهر في صيغة هذه الخلية بغض النظر عن الإشارة إليها أو عدم الرجوع إليها أثناء الحساب.
على سبيل المثال ، على الرغم من عدم استخدام الخلية A2 في الصيغة "= IF (TRUE، A1، A2)" أثناء الحساب ،
لا يزال يعتبر بمثابة سوابق للصيغة. للحصول على تلك المراجع التي تؤثر على الحساب فقط ، يرجى استخدام [Cell.get_precedents_in_calculation()](/cells/ar/python-net/aspose.cells/cell/get_precedents_in_calculation).
###  مثال

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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)

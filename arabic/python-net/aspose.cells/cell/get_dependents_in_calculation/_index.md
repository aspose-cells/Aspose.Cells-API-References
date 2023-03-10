---
title: طريقة get_dependents_in_calculation
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(recursive) {#bool}
يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية.


###  عائدات

العداد لتعداد جميع المعالين (Cell كائن)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| recursive | bool | ما إذا كان يُرجع هؤلاء المعالين الذين لا يشيرون إلى هذه الخلية مباشرةً<br/> لكن بالإشارة إلى أوراق أخرى لهذه الخلية|
###  ملاحظات

لاستخدام هذه الطريقة ، يرجى التأكد من تعيين المصنف بقيمة حقيقية لـ
تم احتساب [FormulaSettings.enable_calculation_chain](/cells/ar/python-net/aspose.cells/formulasettings#enable_calculation_chain) بالكامل باستخدام هذه المحددات.
إذا لم يكن هناك مرجع صيغة لهذه الخلية ، فسيتم إرجاع قيمة خالية.
###  مثال

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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)

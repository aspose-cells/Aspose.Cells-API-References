---
title: طريقة get_precedents_in_calculation
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 190
url: /ar/python-net/aspose.cells/cell/get_precedents_in_calculation/
is_root: false
---
##  get_precedents_in_calculation() {#}
الحصول على جميع السابقات (مرجع إلى الخلايا في المصنف الحالي) المستخدمة بواسطة صيغة هذه الخلية أثناء حسابها.


###  عائدات

عداد لتعداد جميع المراجع (المنطقة المرجعية)


```python
def get_precedents_in_calculation(self):
    ...
```


###  ملاحظات

يمكن أن تعمل هذه الطريقة فقط مع الموقف الذي هو [FormulaSettings.enable_calculation_chain](/cells/ar/python-net/aspose.cells/formulasettings#enable_calculation_chain)
هذا صحيح بالنسبة للمصنف وقد تم حساب المصنف بالكامل.
إذا لم تكن هذه الخلية صيغة أو لا تشير إلى أي خلايا أخرى ، فسيتم إرجاع القيمة الخالية.
###  أمثلة

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



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)

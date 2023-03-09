---
title: طريقة find_formula_contains
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 310
url: /ar/python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---
##  find_formula_contains(formula, previous_cell) {#str-Cell}
يبحث عن الخلية مع الصيغة التي تحتوي على سلسلة الإدخال.


###  عائدات

Cell كائن.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| formula | str | الصيغة للبحث عنها.|
| previous_cell | [Cell](/cells/ar/python-net/aspose.cells/cell) |الخلية السابقة بنفس الصيغة. يمكن تعيين هذه المعلمة على قيمة خالية إذا كان البحث من البداية.|
###  ملاحظات

تُرجع فارغة (لا شيء) إذا لم يتم العثور على خلية.
 ملاحظة: هذا العضو قد عفا عليه الزمن الآن.
الرجاء استخدام Cells.Find (object، Cell، FindOptions) طريقة مع LookInType كـ LookInType.OnlyFormulas
 و LookAtType كـ LookAtType.Contains.
 ستتم إزالة هذا العضو بعد 12 شهرًا منذ نوفمبر 2018.
Aspose يعتذر عن أي إزعاج قد يكون سببه لك.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)

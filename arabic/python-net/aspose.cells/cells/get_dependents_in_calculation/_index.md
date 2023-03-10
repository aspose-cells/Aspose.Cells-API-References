---
title: طريقة get_dependents_in_calculation
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 390
url: /ar/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على خلية معينة.


###  عائدات

العداد لتعداد جميع المعالين (Cell كائن)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| row | int | فهرس صف الخلية المحددة|
| column | int | فهرس العمود للخلية المحددة.|
| recursive | bool | ما إذا كان يُرجع هؤلاء المعالين الذين لا يشيرون إلى الخلية المحددة مباشرةً<br/> لكن بالإشارة إلى أوراق أخرى لتلك الخلية.|
###  ملاحظات

لاستخدام هذه الطريقة ، يرجى التأكد من تعيين المصنف بقيمة حقيقية لـ
تم احتساب [FormulaSettings.enable_calculation_chain](/cells/ar/python-net/aspose.cells/formulasettings#enable_calculation_chain) بالكامل باستخدام هذه المحددات.
إذا لم يكن هناك مرجع صيغة لهذه الخلية ، فسيتم إرجاع قيمة خالية.
لمزيد من التفاصيل والمثال ، يرجى الاطلاع على [Cell.get_dependents_in_calculation(recursive)](/cells/ar/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)

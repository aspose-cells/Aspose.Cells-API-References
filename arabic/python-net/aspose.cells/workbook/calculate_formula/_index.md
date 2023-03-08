---
title: طريقة calculate_formula
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
تحسب نتيجة الصيغ.



```python
def calculate_formula(self):
    ...
```


###  ملاحظات

لجميع الصيغ المدعومة ، يرجى الاطلاع على القائمة على https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

##  calculate_formula(ignore_error) {#bool}

تحسب نتيجة الصيغ.



```python
def calculate_formula(self, ignore_error):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| ignore_error | bool | يشير إلى إخفاء الخطأ في حساب الصيغ. قد يكون الخطأ وظيفة غير مدعومة ، أو روابط خارجية ، إلخ.|


##  calculate_formula(options) {#CalculationOptions}
حساب الصيغ في هذا المصنف.



```python
def calculate_formula(self, options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| options | [CalculationOptions](/cells/ar/python-net/aspose.cells/calculationoptions) | خيارات الحساب|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
تحسب نتيجة الصيغ.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| ignore_error | bool | يشير إلى إخفاء الخطأ في حساب الصيغ. قد يكون الخطأ وظيفة غير مدعومة ، أو روابط خارجية ، إلخ.|
| custom_function | [ICustomFunction](/cells/ar/python-net/aspose.cells/icustomfunction) | وظائف حساب الصيغة المخصصة لتوسيع محرك الحساب.|
###  ملاحظات

ملاحظة: هذا العضو قد عفا عليه الزمن الآن. بدلاً من،
الرجاء استخدام طريقة CalculateFormula (CalculationOptions).
 ستتم إزالة هذه الطريقة بعد 12 شهرًا منذ أغسطس 2020.
Aspose يعتذر عن أي إزعاج قد يكون سببه لك.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)

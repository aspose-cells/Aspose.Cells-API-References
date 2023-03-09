---
title: طريقة set_dynamic_array_formula
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 310
url: /ar/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
يعيّن صيغة صفيف ديناميكية ويجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.


###  عائدات

النطاق الذي يجب أن تمتد إليه الصيغة.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| array_formula | str | تعبير الصيغة|
| options | [FormulaParseOptions](/cells/ar/python-net/aspose.cells/formulaparseoptions) | خيارات لتحليل الصيغة.<br/> سيتم تجاهل خيار "التحليل" وسيتم دائمًا تحليل الصيغة فورًا|
| calculate_value | bool | ما إذا كان سيتم حساب صيغة الصفيف الديناميكية هذه لتلك الخلايا في النطاق الممتد.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
يعيّن صيغة صفيف ديناميكية ويجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.


###  عائدات

النطاق الذي يجب أن تمتد إليه الصيغة.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| array_formula | str | تعبير الصيغة|
| options | [FormulaParseOptions](/cells/ar/python-net/aspose.cells/formulaparseoptions) | خيارات لتحليل الصيغة.<br/> سيتم تجاهل خيار "التحليل" وسيتم دائمًا تحليل الصيغة فورًا|
| values | list |قيم تلك الخلايا مع صيغة صفيف ديناميكية معينة|
| calculate_range | bool | ما إذا كان سيتم حساب النطاق المسكوب لصيغة الصفيف الديناميكية هذه أم لا.<br/>إذا لم تكن معلمة "القيم" خالية وكانت هذه العلامة خاطئة ،<br/> سيكون ارتفاع النطاق المنسكب قيمًا ، وسيكون الطول والعرض قيمتين [0]. الطول.|
| calculate_value | bool | سواء حساب صيغة الصفيف الديناميكية هذه للخلايا في النطاق المسكوب عندما تكون "القيم" خالية<br/> أو العنصر المقابل في "القيم" لخلية واحدة فارغ.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
يعيّن صيغة صفيف ديناميكية ويجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن.


###  عائدات

النطاق الذي يجب أن تمتد إليه الصيغة.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| array_formula | str | تعبير الصيغة|
| options | [FormulaParseOptions](/cells/ar/python-net/aspose.cells/formulaparseoptions) | خيارات لتحليل الصيغة.<br/> سيتم تجاهل خيار "التحليل" وسيتم دائمًا تحليل الصيغة فورًا|
| values | list |قيم تلك الخلايا مع صيغة صفيف ديناميكية معينة|
| calculate_range | bool | ما إذا كان سيتم حساب النطاق المسكوب لصيغة الصفيف الديناميكية هذه أم لا.<br/>إذا لم تكن معلمة "القيم" خالية وكانت هذه العلامة خاطئة ،<br/> سيكون ارتفاع النطاق المنسكب قيمًا ، وسيكون الطول والعرض قيمتين [0]. الطول.|
| calculate_value | bool | سواء حساب صيغة الصفيف الديناميكية هذه للخلايا في النطاق المسكوب عندما تكون "القيم" خالية<br/> أو العنصر المقابل في "القيم" لخلية واحدة فارغ.|
| copts | [CalculationOptions](/cells/ar/python-net/aspose.cells/calculationoptions) | خيارات حساب الصيغة.<br/> بشكل عام ، للنظر في الأداء ، يجب أن تكون الخاصية [CalculationOptions.recursive](/cells/ar/python-net/aspose.cells/calculationoptions#recursive) خطأ.|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cell](/cells/ar/python-net/aspose.cells/cell)

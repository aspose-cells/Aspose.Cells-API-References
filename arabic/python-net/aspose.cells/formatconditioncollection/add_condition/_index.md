---
title: طريقة add_condition
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
أضف شرط تنسيق.


###  عائدات

فهرس كائن شرط التنسيق ؛


```python
def add_condition(self, type):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [FormatConditionType](/cells/ar/python-net/aspose.cells/formatconditiontype) | نوع شرط التنسيق.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
يضيف شرط تنسيق.


###  عائدات

فهرس كائن شرط التنسيق ؛


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [FormatConditionType](/cells/ar/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/ar/python-net/aspose.cells/formatconditiontype) التنسيق الشرطي.<br/> قد يكون أحد أعضاء FormatConditionType.|
| operator_type | [OperatorType](/cells/ar/python-net/aspose.cells/operatortype) | المقارنة [OperatorType](/cells/ar/python-net/aspose.cells/operatortype).<br/> يمكن أن يكون أحد أعضاء OperatorType.|
| formula1 | str | القيمة أو التعبير المرتبط بالتنسيق الشرطي.<br/>إذا بدأت قيمة الإدخال بـ '=' ، فسيتم اعتبارها معادلة.<br/>وإلا سيتم اعتباره كقيمة عادية (نص ، رقم ، منطقي).<br/> بالنسبة للقيمة النصية التي تبدأ بـ '=' ، يمكن للمستخدم إدخالها كصيغة بتنسيق: "= \" = ... \ "".|
| formula2 | str | القيمة أو التعبير المرتبط بالتنسيق الشرطي.<br/>تنسيق الإدخال هو نفسه مع الصيغة 1|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [FormatConditionCollection](/cells/ar/python-net/aspose.cells/formatconditioncollection)
* فئة [FormatConditionType](/cells/ar/python-net/aspose.cells/formatconditiontype)
* فئة [OperatorType](/cells/ar/python-net/aspose.cells/operatortype)

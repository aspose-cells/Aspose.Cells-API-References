---
title: طريقة on_circular
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
قم بتنفيذ هذه الطريقة للقيام بالأعمال عند حساب الصيغ باستخدام مراجع دائرية.


###  عائدات

ما إذا كان محرك الصيغة يحتاج إلى حساب هذه الخلايا بشكل دائري بعد هذا الاستدعاء.
صحيح للسماح لمحرك الصيغة بمتابعة إجراء العمليات الحسابية لهم.
خطأ للسماح لمحرك الصيغة فقط بتمييز هذه الخلايا على أنها محسوبة.


```python
def on_circular(self, circular_cells_data):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator مع عناصر CalculationCell تمثل الخلايا التي<br/> تعتمد على المراجع الدائرية.|
###  ملاحظات

في التطبيق ، قد يقوم المستخدم أيضًا بتعيين القيمة المتوقعة كنتيجة محسوبة
بالنسبة لجزء / كل هذه الخلايا ، لذلك لن يقوم محرك الصيغة بحسابها بشكل متكرر.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [AbstractCalculationMonitor](/cells/ar/python-net/aspose.cells/abstractcalculationmonitor)

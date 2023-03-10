---
title: طريقة process_cell
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
يبدأ في معالجة خلية واحدة.


###  عائدات

ما إذا كانت هذه الخلية بحاجة إلى الاحتفاظ بها في نموذج الخلايا للورقة الحالية.
بشكل عام ، يجب أن يكون خطأ بحيث لا يتم الاحتفاظ بجميع الخلايا في الذاكرة بعد معالجتها ثم يتم حفظ الذاكرة.
لبعض الأغراض الخاصة مثل يحتاج المستخدم إلى الوصول إلى بعض الخلايا لاحقًا بعد معالجة المصنف بأكمله ،
يمكن للمستخدم أن يجعل هذه الطريقة تعود بشكل صحيح للحفاظ على تلك الخلايا الخاصة في نموذج Cells والوصول إليها لاحقًا بواسطة واجهات برمجة التطبيقات مثل Cells [صف ، عمود].
ومع ذلك ، فإن الاحتفاظ ببيانات الخلايا في نموذج Cells يتطلب المزيد من الذاكرة وإذا تم الاحتفاظ بجميع الخلايا ، فقم بقراءة ملف القالب
في وضع LightCells سيصبح مثل قراءته بالطريقة العادية.


```python
def process_cell(self, cell):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| cell | [Cell](/cells/ar/python-net/aspose.cells/cell) | Cell العنصر الذي يتم تشغيله حاليا|
###  ملاحظات

سيتم استدعاؤه بعد قراءة بيانات خلية واحدة.


###  أنظر أيضا

* وحدة [aspose.cells](../../)
* فئة [LightCellsDataHandler](/cells/ar/python-net/aspose.cells/lightcellsdatahandler)

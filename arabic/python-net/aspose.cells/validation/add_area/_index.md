---
title: طريقة add_area
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
يطبق التحقق على المنطقة.



```python
def add_area(self, cell_area):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| cell_area | [CellArea](/cells/ar/python-net/aspose.cells/cellarea) | المنطقة.|
###  ملاحظات

يكافئ استخدام [Validation.add_area(cell_area)](/cells/ar/python-net/aspose.cells/validation/add_area)
مع فحص التقاطع والحافة.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
يطبق التحقق على المنطقة.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| cell_area | [CellArea](/cells/ar/python-net/aspose.cells/cellarea) | المنطقة.|
| check_intersection | bool | سواء تحقق من تقاطع منطقة معينة مع مناطق التحقق الموجودة.<br/>إذا تم تطبيق تحقق واحد في منطقة معينة (أو جزء منها) ،<br/>ثم يجب إزالة التحقق الحالي في البداية من منطقة معينة.<br/>وإلا فقد يحدث تلف لعمليات التحقق التي تم إنشاؤها.<br/>إذا كان المستخدم متأكدًا من أن المنطقة المضافة لا تتقاطع مع أي منطقة موجودة ،<br/> يمكن تعيين هذا المعامل كخطأ لاعتبارات الأداء.|
| check_edge | bool | سواء تحقق من حافة المناطق المطبقة في هذا التحقق من الصحة.<br/>تعتمد الإعدادات الداخلية للتحقق من الصحة على أعلى يسار أحد نطاقاتها المطبقة ،<br/>لذلك إذا كانت منطقة معينة ستصبح المنطقة الجديدة العلوية اليسرى من النطاقات المطبقة ،<br/>يجب تغيير الإعدادات الداخلية وإعادة بنائها ، وإلا فقد يحدث نتيجة غير متوقعة.<br/>إذا كان المستخدم متأكدًا من أن المنطقة المضافة ليست المنطقة العلوية اليسرى ،<br/> يمكن تعيين هذا المعامل كخطأ لاعتبارات الأداء.|
###  ملاحظات

في هذه الطريقة ، سنزيل جميع عمليات التحقق القديمة في منطقة معينة.
بالنسبة إلى النطاق العلوي الأيسر من النطاقات المطبقة في التحقق من الصحة ، يكون StartRow أولاً هو الأصغر ،
ثانيًا ، يعد StartColumn الخاص به هو أصغر منطقة من تلك المناطق التي لديها نفس StartRow الأصغر.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Validation](/cells/ar/python-net/aspose.cells/validation)

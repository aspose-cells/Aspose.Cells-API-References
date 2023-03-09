---
title: طريقة remove_at
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells/externallinkcollection/remove_at/
is_root: false
---
##  remove_at(index) {#int}
يزيل الارتباط الخارجي المحدد من المصنف.



```python
def remove_at(self, index):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| index | int | فهرس الارتباط الخارجي المراد إزالته.|
###  ملاحظات

عند إزالة الارتباط الخارجي ، ستتم أيضًا إزالة جميع الصيغ التي تشير إليه بسبب
تصبح المراجع غير صالحة.

##  remove_at(index, update_references_as_local) {#int-bool}
يزيل الارتباط الخارجي المحدد من المصنف.



```python
def remove_at(self, index, update_references_as_local):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| index | int | فهرس الارتباط الخارجي المراد إزالته.|
| update_references_as_local | bool | ما إذا كان يتم تحديث كافة المراجع الخاصة بالارتباط الخارجي المعطى لمرجع المصنف الحالي نفسه.|
###  ملاحظات

إذا كانت المراجع مطلوبة للتحديث ، فسيتم تغيير المراجع إلى الارتباطات الخارجية في الصيغ إلى المصنف الحالي.
على سبيل المثال ، الرابط الخارجي المراد إزالته هو "externalsource.xlam" ويحدد وظيفة مخصصة واحدة "customfunction ()" ،
الصيغة الأصلية لخلية واحدة هي "= 'externalsource.xlam'! customfunction ()" ،
بعد إزالة الصيغة ستصبح "= customfunction ()".
إذا لم تكن هناك حاجة إلى تحديث المراجع ، فكل الصيغ التي تشير إلى هذا الارتباط الخارجي
ستتم إزالتها أيضًا لأن هذه المراجع تصبح غير صالحة.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [ExternalLinkCollection](/cells/ar/python-net/aspose.cells/externallinkcollection)

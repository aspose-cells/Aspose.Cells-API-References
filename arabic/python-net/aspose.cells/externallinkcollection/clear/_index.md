---
title: طريقة clear
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 30
url: /ar/python-net/aspose.cells/externallinkcollection/clear/
is_root: false
---
##  clear() {#}
يزيل كل الروابط الخارجية.



```python
def clear(self):
    ...
```


###  ملاحظات

عند إزالة الروابط الخارجية ، ستتم أيضًا إزالة جميع الصيغ التي تشير إليها بسبب
تصبح المراجع غير صالحة.

##  clear(update_references_as_local) {#bool}
يزيل كل الروابط الخارجية.



```python
def clear(self, update_references_as_local):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| update_references_as_local | bool | ما إذا كان يتم تحديث كافة مراجع الارتباطات الخارجية كمراجع للمصنف الحالي نفسه.|
###  ملاحظات

إذا كانت المراجع مطلوبة للتحديث ، فسيتم تغيير المراجع إلى الارتباطات الخارجية في الصيغ إلى المصنف الحالي.
على سبيل المثال ، الصيغة الأصلية لخلية واحدة هي "= 'externalsource.xlam'! customfunction ()" ،
بعد إزالة الروابط الخارجية ، ستصبح الصيغة "= customfunction ()".
إذا لم يكن مطلوبًا تحديث المراجع ، فكل الصيغ التي تحتوي على مراجع إلى ارتباطات خارجية
ستتم إزالتها أيضًا لأن هذه المراجع تصبح غير صالحة.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [ExternalLinkCollection](/cells/ar/python-net/aspose.cells/externallinkcollection)

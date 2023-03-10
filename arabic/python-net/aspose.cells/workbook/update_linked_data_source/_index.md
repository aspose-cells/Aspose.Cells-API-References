---
title: طريقة update_linked_data_source
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 410
url: /ar/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
إذا احتوى هذا المصنف على ارتباطات خارجية بمصدر بيانات آخر ،
Aspose.Cells سيحاول استرجاع أحدث البيانات.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| external_workbooks | list | يتم الرجوع إلى المصنفات الخارجية بواسطة هذا المصنف.<br/>إذا كانت فارغة ، فسنفتح الملفات المرتبطة الخارجية مباشرة ..<br/> إذا لم يكن فارغًا ،<br/>سوف نتحقق مما إذا كان الرابط الخارجي في المصفوفة أولاً ؛<br/> إذا لم يكن كذلك ، فسنفتح الملفات المرتبطة الخارجية مرة أخرى.|
###  ملاحظات

إذا لم يتم استدعاء الطريقة قبل حساب الصيغ ،
Aspose.Cells سوف يستخدم المعلومات السابقة (المخبأة في الملف) ؛
 يرجى تعيين CellsHelper.StartupPath ، CellsHelper.AltStartPath ، CellsHelper.LibraryPath.
ويرجى تعيين Workbook.FilePath إذا كان هذا المصنف من دفق ،
وإلا فلن يتمكن Aspose.Cells من الحصول على المسار الكامل للوصلة الخارجية في بعض الأحيان.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)

---
title: multi_thread_reading الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1200
url: /ar/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading الملكية

الحصول على أو تحديد ما إذا كان يجب أن يدعم نموذج بيانات الخلايا القراءة متعددة الخيوط.
القيمة الافتراضية لهذه الخاصية خاطئة.

###  ملاحظات

إذا كان هناك العديد من سلاسل الرسائل لقراءة عناصر الصف / Cell في هذه المجموعة بشكل متزامن ،
يجب تعيين هذه الخاصية على أنها true ، وإلا فقد يتم إنتاج نتيجة غير متوقعة.
قد يؤدي دعم القراءة متعددة الخيوط إلى تدهور أداء الوصول إلى كائنات الصف / Cell من هذه المجموعة.
يرجى ملاحظة أن بعض الميزات لا يمكن أن تدعم قراءة Multi-Thread ،
مثل قيم التنسيق (بواسطة [Cell.string_value](/cells/ar/python-net/aspose.cells/cell#string_value) ، [Cell.display_string_value](/cells/ar/python-net/aspose.cells/cell#display_string_value) ، إلخ.).
لذلك ، حتى مع تعيين هذه الخاصية على أنها صحيحة ، قد لا تزال واجهات برمجة التطبيقات هذه تعطي نتيجة غير متوقعة لقراءة Multi-Thread.
###  تعريف:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Cells](/cells/ar/python-net/aspose.cells/cells)

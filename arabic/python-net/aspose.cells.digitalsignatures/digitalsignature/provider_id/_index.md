---
title: provider_id الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
##  provider_id الملكية

يحدد معرف فئة موفر التوقيع.
القيمة الافتراضية هي فارغة (جميع الأصفار).

###  ملاحظات

موفر خدمة التشفير (CSP) هو وحدة برمجية مستقلة تقوم بالفعل بتنفيذ خوارزميات التشفير للمصادقة والتشفير والتشفير.
Microsoft يحتفظ Office بقيمة {00000000-0000-0000-0000-000000000000} لموفر التوقيع الافتراضي الخاص به ،
و {000CD6A4-0000-0000-C000-000000000046} لموفر التوقيع من شرق آسيا.

يجب الحصول على المعرف الفريد العمومي (GUID) الخاص بالموفر المثبت بشكل إضافي من الوثائق التي يتم شحنها مع الموفر.
###  تعريف:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.digitalsignatures](../../)
* فئة [DigitalSignature](/cells/ar/python-net/aspose.cells.digitalsignatures/digitalsignature)

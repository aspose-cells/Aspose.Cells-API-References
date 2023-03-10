---
title: provider_id الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 80
url: /ar/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id الملكية

الحصول على معرف موفر التوقيع وتعيينه.

###  ملاحظات

عادةً ما يكون هو CLSID الخاص بالوظيفة الإضافية الخاصة بالموفر.

###  مثال

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
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
* وحدة [aspose.cells.drawing](../../)
* فئة [SignatureLine](/cells/ar/python-net/aspose.cells.drawing/signatureline)

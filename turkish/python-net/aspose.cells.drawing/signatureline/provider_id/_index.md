---
title: provider_id mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 80
url: /tr/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id mülk

İmza sağlayıcının kimliğini alır ve ayarlar.

###  Notlar

Genellikle sağlayıcı com eklentisinin CLSID'sidir.

###  Örnek

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
###  Tanım:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [SignatureLine](/cells/tr/python-net/aspose.cells.drawing/signatureline)

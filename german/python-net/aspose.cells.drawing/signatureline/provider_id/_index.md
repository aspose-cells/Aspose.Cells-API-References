---
title: provider_id Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 80
url: /de/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id Eigentum

Ruft die ID des Signaturanbieters ab und legt sie fest.

###  Bemerkungen

Dies ist in der Regel die CLSID des Provider-COM-Add-Ins.

###  Beispiel

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
###  Definition:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [SignatureLine](/cells/de/python-net/aspose.cells.drawing/signatureline)

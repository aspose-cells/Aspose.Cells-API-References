---
title: provider_id fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 80
url: /sv/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id fastighet

Hämtar och ställer in id för signaturleverantör.

###  Anmärkningar

Det är vanligtvis CLSID för provider com-tillägget.

###  Exempel

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

###  Se även
* modul [aspose.cells.drawing](../../)
* klass [SignatureLine](/cells/sv/python-net/aspose.cells.drawing/signatureline)

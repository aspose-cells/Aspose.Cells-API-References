---
title: provider_id proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 80
url: /it/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id proprietà

Ottiene e imposta l'ID del provider di firme.

###  Osservazioni

In genere è il CLSID del componente aggiuntivo com del provider.

###  Esempio

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
###  Definizione:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [SignatureLine](/cells/it/python-net/aspose.cells.drawing/signatureline)

---
title: provider_id propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 80
url: /fr/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id propriété

Obtient et définit l'ID du fournisseur de signature.

###  Remarques

Il s'agit généralement du CLSID du complément com du fournisseur.

###  Exemple

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
###  Définition:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [SignatureLine](/cells/fr/python-net/aspose.cells.drawing/signatureline)

---
title: provider_id propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 80
url: /es/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
##  provider_id propiedad

Obtiene y establece la identificación del proveedor de la firma.

###  Observaciones

Por lo general, es el CLSID del complemento com del proveedor.

###  Ejemplo

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
###  Definición:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [SignatureLine](/cells/es/python-net/aspose.cells.drawing/signatureline)

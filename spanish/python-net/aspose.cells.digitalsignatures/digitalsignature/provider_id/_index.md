---
title: provider_id propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
##  provider_id propiedad

Especifica el ID de clase del proveedor de firmas.
El valor predeterminado es GUID vacío (todo ceros).

###  Observaciones

El proveedor de servicios criptográficos (CSP) es un módulo de software independiente que en realidad ejecuta algoritmos criptográficos para autenticación, codificación y encriptación.
Microsoft Office reserva el valor de {00000000-0000-0000-0000-000000000000} para su proveedor de firma predeterminado,
y {000CD6A4-0000-0000-C000-000000000046} para su proveedor de firmas de Asia oriental.

El GUID del proveedor instalado adicionalmente debe obtenerse de la documentación enviada con el proveedor.
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
* módulo [aspose.cells.digitalsignatures](../../)
* clase [DigitalSignature](/cells/es/python-net/aspose.cells.digitalsignatures/digitalsignature)

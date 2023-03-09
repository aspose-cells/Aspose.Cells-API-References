---
title: VbaProject clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  VbaProject clase
Representa el proyecto VBA.



El tipo VbaProject expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [is_valid_signed](/cells/es/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Indica si la firma del proyecto VBA es válida o no.|
| [cert_raw_data](/cells/es/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Obtiene datos sin procesar del certificado si este proyecto de VBA está firmado.|
| [name](/cells/es/python-net/aspose.cells.vba/vbaproject/name) | Obtiene y establece el nombre del proyecto de VBA.|
| [is_signed](/cells/es/python-net/aspose.cells.vba/vbaproject/is_signed) | Indica si VBAcode está firmado o no.|
| [is_protected](/cells/es/python-net/aspose.cells.vba/vbaproject/is_protected) | Indica si este proyecto de VBA está protegido.|
| [islocked_for_viewing](/cells/es/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Indica si este proyecto de VBA está bloqueado para su visualización.|
| [modules](/cells/es/python-net/aspose.cells.vba/vbaproject/modules) | Obtiene todos los objetos [VbaModule](/cells/es/python-net/aspose.cells.vba/vbamodule).|
| [references](/cells/es/python-net/aspose.cells.vba/vbaproject/references) | Obtiene todas las referencias del proyecto VBA.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [sign(digital_signature)](/cells/es/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Firme este proyecto de VBA con una firma digital|
| [protect(islocked_for_viewing, password)](/cells/es/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Protege o desprotege este proyecto de VBA.|
| [copy(source)](/cells/es/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Copie el proyecto VBA de otro archivo.|
| [validate_password(password)](/cells/es/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Valida contraseña de protección.|



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.vba](..)
* clase [VbaModule](/cells/es/python-net/aspose.cells.vba/vbamodule)

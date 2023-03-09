---
title: VbaProjectReference clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference clase
Representa la referencia del proyecto VBA.



El tipo VbaProjectReference expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [type](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/type) | Obtiene el tipo de esta referencia.|
| [name](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/name) | Obtiene y establece el nombre de la referencia.|
| [libid](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/libid) | Obtiene y establece la Libid de la referencia.|
| [twiddledlibid](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Obtiene y establece la Libid alterada de la referencia.|
| [extended_libid](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Obtiene y establece la Libid extendida de la referencia.|
| [relative_libid](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) |Obtiene y establece el identificador del proyecto VBA al que se hace referencia con una ruta relativa.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [copy(source)](/cells/es/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ver también
* módulo [aspose.cells.vba](..)

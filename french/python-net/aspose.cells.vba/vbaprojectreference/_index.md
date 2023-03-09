---
title: VbaProjectReference classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference classe
Représente la référence du projet VBA.



Le type VbaProjectReference expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [type](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/type) | Obtient le type de cette référence.|
| [name](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/name) | Obtient et définit le nom de la référence.|
| [libid](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/libid) | Obtient et définit la Libid de la référence.|
| [twiddledlibid](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) | Obtient et définit la Libid tordue de la référence.|
| [extended_libid](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) | Obtient et définit la Libid étendue de la référence.|
| [relative_libid](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) |Obtient et définit l'identifiant du projet VBA référencé avec un chemin relatif.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [copy(source)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



###  Exemple

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

###  Voir également
* module [aspose.cells.vba](..)

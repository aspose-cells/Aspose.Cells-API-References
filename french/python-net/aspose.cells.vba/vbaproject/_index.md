---
title: VbaProject classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  VbaProject classe
Représente le projet VBA.



Le type VbaProject expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_valid_signed](/cells/fr/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Indique si la signature du projet VBA est valide ou non.|
| [cert_raw_data](/cells/fr/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Obtient les données brutes du certificat si ce projet VBA est signé.|
| [name](/cells/fr/python-net/aspose.cells.vba/vbaproject/name) | Obtient et définit le nom du projet VBA.|
| [is_signed](/cells/fr/python-net/aspose.cells.vba/vbaproject/is_signed) | Indique si VBAcode est signé ou non.|
| [is_protected](/cells/fr/python-net/aspose.cells.vba/vbaproject/is_protected) | Indique si ce projet VBA est protégé.|
| [islocked_for_viewing](/cells/fr/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Indique si ce projet VBA est verrouillé pour l'affichage.|
| [modules](/cells/fr/python-net/aspose.cells.vba/vbaproject/modules) | Obtient tous les objets [VbaModule](/cells/fr/python-net/aspose.cells.vba/vbamodule).|
| [references](/cells/fr/python-net/aspose.cells.vba/vbaproject/references) | Obtient toutes les références du projet VBA.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [sign(digital_signature)](/cells/fr/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Signez ce projet VBA par une signature numérique|
| [protect(islocked_for_viewing, password)](/cells/fr/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Protège ou déprotége ce projet VBA.|
| [copy(source)](/cells/fr/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Copiez le projet VBA à partir d'un autre fichier.|
| [validate_password(password)](/cells/fr/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Valide le mot de passe de protection.|



###  Exemples

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Voir également
* module [aspose.cells.vba](..)
* classe [VbaModule](/cells/fr/python-net/aspose.cells.vba/vbamodule)

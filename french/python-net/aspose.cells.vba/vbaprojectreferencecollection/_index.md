---
title: VbaProjectReferenceCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 50
url: /fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/
is_root: false
---
##  VbaProjectReferenceCollection classe
Représente toutes les références du projet VBA.



Le type VbaProjectReferenceCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [copy_to(array)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/index_of/#VbaProjectReference-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/last_index_of/#VbaProjectReference-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [add_registered_reference(name, libid)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_registered_reference/#str-str) | Ajoutez une référence à une bibliothèque de types Automation.|
| [add_control_refrernce(name, libid, twiddledlibid, extended_libid)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_control_refrernce/#str-str-str-str) | Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue.|
| [add_project_refrernce(name, absolute_libid, relative_libid)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/add_project_refrernce/#str-str-str) | Ajoute une référence à un projet VBA externe.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.vba/vbaprojectreferencecollection/binary_search/#VbaProjectReference) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



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

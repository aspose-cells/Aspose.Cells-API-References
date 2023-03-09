---
title: ExternalLinkCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 570
url: /fr/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  ExternalLinkCollection classe
Représente la collection de liens externes dans un classeur.



Le type ExternalLinkCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [count](/cells/fr/python-net/aspose.cells/externallinkcollection/count) | Obtient le nombre d'éléments réellement contenus dans la collection.|



Obtient l'élément [ExternalLink](/cells/fr/python-net/aspose.cells/externallink) à l'index spécifié.
###  Indexeur
| Nom| Description|
| :- | :- |
| [index] | Index de base zéro de l'élément.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(file_name, sheet_names)](/cells/fr/python-net/aspose.cells/externallinkcollection/add/#str-list) | Ajoute un lien externe.|
| [add(directory_type, file_name, sheet_names)](/cells/fr/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | Ajouter un lien externe .|
| [clear()](/cells/fr/python-net/aspose.cells/externallinkcollection/clear/#) | Supprime tous les liens externes.|
| [clear(update_references_as_local)](/cells/fr/python-net/aspose.cells/externallinkcollection/clear/#bool) | Supprime tous les liens externes.|
| [remove_at(index)](/cells/fr/python-net/aspose.cells/externallinkcollection/remove_at/#int) | Supprime le lien externe spécifié du classeur.|
| [remove_at(index, update_references_as_local)](/cells/fr/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | Supprime le lien externe spécifié du classeur.|



###  Exemple

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  Voir également
* module [aspose.cells](..)
* classe [ExternalLink](/cells/fr/python-net/aspose.cells/externallink)

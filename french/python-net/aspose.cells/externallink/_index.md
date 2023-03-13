---
title: ExternalLink classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 560
url: /fr/python-net/aspose.cells/externallink/
is_root: false
---
##  ExternalLink classe
Représente un lien externe dans un classeur.



Le type ExternalLink expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [type](/cells/fr/python-net/aspose.cells/externallink/type) | Obtient le type de lien externe.|
| [original_data_source](/cells/fr/python-net/aspose.cells/externallink/original_data_source) | Représente la source de données stockée du lien externe.|
| [data_source](/cells/fr/python-net/aspose.cells/externallink/data_source) | Représente la source de données du lien externe.|
| [is_referred](/cells/fr/python-net/aspose.cells/externallink/is_referred) | Indique si ce lien externe est référencé par d'autres.|
| [is_visible](/cells/fr/python-net/aspose.cells/externallink/is_visible) | Indique si ce lien externe est visible dans MS Excel.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/fr/python-net/aspose.cells/externallink/add_external_name/#str-str) | Ajoute un nom externe.|



###  Exemple

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  Voir également
* module [aspose.cells](..)

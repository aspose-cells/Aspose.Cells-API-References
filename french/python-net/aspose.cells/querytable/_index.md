---
title: QueryTable classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1230
url: /fr/python-net/aspose.cells/querytable/
is_root: false
---
##  QueryTable classe
Représente les informations QueryTable.



Le type QueryTable expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [connection_id](/cells/fr/python-net/aspose.cells/querytable/connection_id) | Obtient l'ID de connexion de la table de requête.|
| [external_connection](/cells/fr/python-net/aspose.cells/querytable/external_connection) | Obtient la connexion externe associée.|
| [name](/cells/fr/python-net/aspose.cells/querytable/name) | Obtient le nom de la table de requête.|
| [result_range](/cells/fr/python-net/aspose.cells/querytable/result_range) | Obtient la plage du résultat.|
| [preserve_formatting](/cells/fr/python-net/aspose.cells/querytable/preserve_formatting) | Renvoie ou définit le PreserveFormatting de l'objet.|
| [adjust_column_width](/cells/fr/python-net/aspose.cells/querytable/adjust_column_width) | Renvoie ou définit la AdjustColumnWidth de l'objet.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Getting the first query table in the worksheet
qt = worksheet.query_tables[0]
# Getting display address of the query table.
address = qt.result_range.address

```

###  Voir également
* module [aspose.cells](..)

---
title: QueryTable Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1230
url: /de/python-net/aspose.cells/querytable/
is_root: false
---
##  QueryTable Klasse
Stellt QueryTable-Informationen dar.



Der Typ QueryTable macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [connection_id](/cells/de/python-net/aspose.cells/querytable/connection_id) | Ruft die Verbindungs-ID der Abfragetabelle ab.|
| [external_connection](/cells/de/python-net/aspose.cells/querytable/external_connection) | Ruft die zugehörige externe Verbindung ab.|
| [name](/cells/de/python-net/aspose.cells/querytable/name) | Ruft den Namen der Abfragetabelle ab.|
| [result_range](/cells/de/python-net/aspose.cells/querytable/result_range) | Ruft den Bereich des Ergebnisses ab.|
| [preserve_formatting](/cells/de/python-net/aspose.cells/querytable/preserve_formatting) | Gibt die PreserveFormatting des Objekts zurück oder legt sie fest.|
| [adjust_column_width](/cells/de/python-net/aspose.cells/querytable/adjust_column_width) | Gibt die AdjustColumnWidth des Objekts zurück oder legt sie fest.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)

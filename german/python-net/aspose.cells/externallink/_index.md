---
title: ExternalLink Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 560
url: /de/python-net/aspose.cells/externallink/
is_root: false
---
##  ExternalLink Klasse
Stellt einen externen Link in einer Arbeitsmappe dar.



Der Typ ExternalLink macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [type](/cells/de/python-net/aspose.cells/externallink/type) | Ruft den Typ des externen Links ab.|
| [original_data_source](/cells/de/python-net/aspose.cells/externallink/original_data_source) | Repräsentiert die gespeicherte Datenquelle des externen Links.|
| [data_source](/cells/de/python-net/aspose.cells/externallink/data_source) | Stellt die Datenquelle des externen Links dar.|
| [is_referred](/cells/de/python-net/aspose.cells/externallink/is_referred) | Gibt an, ob auf diesen externen Link von anderen verwiesen wird.|
| [is_visible](/cells/de/python-net/aspose.cells/externallink/is_visible) | Gibt an, ob dieser externe Link in MS Excel sichtbar ist.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/de/python-net/aspose.cells/externallink/add_external_name/#str-str) | Fügt einen externen Namen hinzu.|



###  Beispiele

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  Siehe auch
* Modul [aspose.cells](..)

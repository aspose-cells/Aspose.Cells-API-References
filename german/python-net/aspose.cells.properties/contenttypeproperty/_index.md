---
title: ContentTypeProperty Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
##  ContentTypeProperty Klasse
Stellt Kennungsinformationen dar.



Der Typ ContentTypeProperty macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [name](/cells/de/python-net/aspose.cells.properties/contenttypeproperty/name) | Gibt den Namen des Objekts zurück oder legt ihn fest.|
| [value](/cells/de/python-net/aspose.cells.properties/contenttypeproperty/value) | Gibt den Wert der Eigenschaft des Inhaltstyps zurück oder legt ihn fest.|
| [type](/cells/de/python-net/aspose.cells.properties/contenttypeproperty/type) | Ruft den Typ der Eigenschaft ab und legt ihn fest.|
| [is_nillable](/cells/de/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Gibt an, ob der Wert leer sein könnte.|



###  Beispiele

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Siehe auch
* Modul [aspose.cells.properties](..)

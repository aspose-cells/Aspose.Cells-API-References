---
title: FindOptions Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 630
url: /de/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions Klasse
Repräsentiert Suchoptionen.



Der Typ FindOptions macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [FindOptions()](/cells/de/python-net/aspose.cells/findoptions/__init__/#) | Erstellt eine neue Instanz von FindOptions|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_case_sensitive](/cells/de/python-net/aspose.cells/findoptions/is_case_sensitive) | Gibt an, ob bei der gesuchten Zeichenfolge zwischen Groß- und Kleinschreibung unterschieden wird.|
| [case_sensitive](/cells/de/python-net/aspose.cells/findoptions/case_sensitive) | Gibt an, ob bei der gesuchten Zeichenfolge zwischen Groß- und Kleinschreibung unterschieden wird.|
| [look_at_type](/cells/de/python-net/aspose.cells/findoptions/look_at_type) | Typ anschauen.|
| [is_range_set](/cells/de/python-net/aspose.cells/findoptions/is_range_set) | Gibt an, ob der gesuchte Bereich festgelegt ist.|
| [search_next](/cells/de/python-net/aspose.cells/findoptions/search_next) | Suchreihenfolge. True: Weitersuchen. False: Vorherige suchen.|
| [search_backward](/cells/de/python-net/aspose.cells/findoptions/search_backward) | Ob rückwärts nach Zellen suchen.|
| [seach_order_by_rows](/cells/de/python-net/aspose.cells/findoptions/seach_order_by_rows) | Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt.|
| [look_in_type](/cells/de/python-net/aspose.cells/findoptions/look_in_type) | Suchen Sie in Typ.|
| [regex_key](/cells/de/python-net/aspose.cells/findoptions/regex_key) | Gibt an, ob es sich bei dem gesuchten Schlüssel um Regex handelt.<br/> Wenn wahr, wird der gesuchte Schlüssel als Regex genommen und geparst. Andernfalls wird der Schlüssel gemäß den Regeln in MS Excel geparst.|
| [value_type_sensitive](/cells/de/python-net/aspose.cells/findoptions/value_type_sensitive) | Gibt an, ob der Werttyp der gesuchten Zelle mit dem gesuchten Schlüssel identisch sein soll.|
| [style](/cells/de/python-net/aspose.cells/findoptions/style) | Das zu suchende Format.|
| [convert_numeric_data](/cells/de/python-net/aspose.cells/findoptions/convert_numeric_data) | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der gesuchte Zeichenfolgenwert in numerische Daten konvertiert wird.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get_range()](/cells/de/python-net/aspose.cells/findoptions/get_range/#) | Ruft den durchsuchten Bereich ab und legt ihn fest.|
| [set_range(ca)](/cells/de/python-net/aspose.cells/findoptions/set_range/#CellArea) | Legt den Suchbereich fest.|



###  Beispiel

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Siehe auch
* Modul [aspose.cells](..)

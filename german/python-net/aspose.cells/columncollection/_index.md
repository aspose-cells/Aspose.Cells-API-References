---
title: ColumnCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 270
url: /de/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection Klasse
Sammlung der [Column](/cells/de/python-net/aspose.cells/column)-Objekte, die die einzelnen Spalten(einstellungen) in einem Arbeitsblatt darstellen.
Das Column-Objekt repräsentiert nur die Einstellungen wie Spaltenbreite, Stile usw. für die ganze Spalte,
hat nichts damit zu tun, dass es nicht leere Zellen (Daten) oder nicht in der entsprechenden Spalte gibt.
Und die "Anzahl" dieser Sammlung stellt nur die Anzahl der Spaltenobjekte dar, die in dieser Sammlung instanziiert wurden.
hat nichts damit zu tun, dass es nicht leere Zellen (Daten) oder nicht im Arbeitsblatt gibt.



Der Typ ColumnCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells/columncollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [copy_to(array)](/cells/de/python-net/aspose.cells/columncollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) | Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/columncollection/index_of/#Column-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/columncollection/last_index_of/#Column) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/columncollection/last_index_of/#Column-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [get_by_index(index)](/cells/de/python-net/aspose.cells/columncollection/get_by_index/#int) | Ruft das Spaltenobjekt nach dem Index ab.|
| [get_column_by_index(index)](/cells/de/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Ruft das Objekt [Column](/cells/de/python-net/aspose.cells/column) anhand der Position in der Liste ab.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/columncollection/binary_search/#Column) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiel

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Column](/cells/de/python-net/aspose.cells/column)

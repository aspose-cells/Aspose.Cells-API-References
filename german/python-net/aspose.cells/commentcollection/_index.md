---
title: CommentCollection Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 290
url: /de/python-net/aspose.cells/commentcollection/
is_root: false
---
##  CommentCollection Klasse
Kapselt eine Sammlung von [Comment](/cells/de/python-net/aspose.cells/comment)-Objekten.



Der Typ CommentCollection macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [capacity](/cells/de/python-net/aspose.cells/commentcollection/capacity) | Ruft die Anzahl der Elemente ab, die die Arrayliste enthalten kann, oder legt diese fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [add_threaded_comment(row, column, text, author)](/cells/de/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-str-ThreadedCommentAuthor) | Fügt einen Thread-Kommentar hinzu.|
| [add_threaded_comment(cell_name, text, author)](/cells/de/python-net/aspose.cells/commentcollection/add_threaded_comment/#str-str-ThreadedCommentAuthor) | Fügt einen Thread-Kommentar hinzu.|
| [get_threaded_comments(row, column)](/cells/de/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Ruft die Thread-Kommentare nach Zeilen- und Spaltenindex ab.|
| [get_threaded_comments(cell_name)](/cells/de/python-net/aspose.cells/commentcollection/get_threaded_comments/#str) | Ruft die Thread-Kommentare nach Zellname ab.|
| [add(row, column)](/cells/de/python-net/aspose.cells/commentcollection/add/#int-int) | Fügt der Sammlung einen Kommentar hinzu.|
| [add(cell_name)](/cells/de/python-net/aspose.cells/commentcollection/add/#str) | Fügt der Sammlung einen Kommentar hinzu.|
| [remove_at(cell_name)](/cells/de/python-net/aspose.cells/commentcollection/remove_at/#str) | Entfernt den Kommentar der bestimmten Zelle.|
| [remove_at(row, column)](/cells/de/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Entfernt den Kommentar der bestimmten Zelle.|
| [copy_to(array)](/cells/de/python-net/aspose.cells/commentcollection/copy_to/#list) | Kopiert die gesamte Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am Anfang der Ziel-Array-Liste.|
| [copy_to(index, array, array_index, count)](/cells/de/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) |Kopiert eine Reihe von Elementen aus der Array-Liste in eine kompatible eindimensionale Array-Liste, beginnend am angegebenen Index der Ziel-Array-Liste.|
| [index_of(item, index)](/cells/de/python-net/aspose.cells/commentcollection/index_of/#Comment-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom angegebenen Index bis zum letzten Element erstreckt.|
| [index_of(item, index, count)](/cells/de/python-net/aspose.cells/commentcollection/index_of/#Comment-int-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des ersten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der am angegebenen Index beginnt und die angegebene Anzahl von Elementen enthält.|
| [last_index_of(item)](/cells/de/python-net/aspose.cells/commentcollection/last_index_of/#Comment) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens in der gesamten Array-Liste zurück.|
| [last_index_of(item, index)](/cells/de/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int) | Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der sich vom ersten Element bis zum angegebenen Index erstreckt.|
| [last_index_of(item, index, count)](/cells/de/python-net/aspose.cells/commentcollection/last_index_of/#Comment-int-int) |Sucht nach dem angegebenen Objekt und gibt den nullbasierten Index des letzten Vorkommens innerhalb des Bereichs von Elementen in der Arrayliste zurück, der die angegebene Anzahl von Elementen enthält und am angegebenen Index endet.|
| [binary_search(item)](/cells/de/python-net/aspose.cells/commentcollection/binary_search/#Comment) | Durchsucht die gesamte sortierte Array-Liste mithilfe des Standardvergleichs nach einem Element und gibt den nullbasierten Index des Elements zurück.|



###  Beispiele

```python
from aspose.cells import Workbook

workbook = Workbook()
comments = workbook.worksheets[0].comments

```

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Comment](/cells/de/python-net/aspose.cells/comment)

---
title: get_threaded_comments Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 60
url: /de/python-net/aspose.cells/commentcollection/get_threaded_comments/
is_root: false
---
##  get_threaded_comments(cell_name) {#str}
Ruft die Thread-Kommentare nach Zellname ab.


###  Kehrt zurück




```python
def get_threaded_comments(self, cell_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| cell_name | str | Der Name der Zelle.|

###  Beispiele

```python

threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
    tc = threadedComments2[i]
    note = tc.notes

```


##  get_threaded_comments(row, column) {#int-int}
Ruft die Thread-Kommentare nach Zeilen- und Spaltenindex ab.


###  Kehrt zurück




```python
def get_threaded_comments(self, row, column):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| row | int | Der Zeilenindex.|
| column | int | Der Spaltenindex.|

###  Beispiele

```python

threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
    tc = threadedComments1[i]
    note = tc.notes

```



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [CommentCollection](/cells/de/python-net/aspose.cells/commentcollection)

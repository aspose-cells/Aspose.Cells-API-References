---
title: get_threaded_comments metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells/commentcollection/get_threaded_comments/
is_root: false
---
##  get_threaded_comments(cell_name) {#str}
Får de trådade kommentarerna efter cellnamn.


###  Returnerar




```python
def get_threaded_comments(self, cell_name):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| cell_name | str | Namnet på cellen.|

###  Exempel

```python

threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
    tc = threadedComments2[i]
    note = tc.notes

```


##  get_threaded_comments(row, column) {#int-int}
Får de trådade kommentarerna efter rad- och kolumnindex.


###  Returnerar




```python
def get_threaded_comments(self, row, column):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| row | int | Radindex.|
| column | int | Kolumnindex.|

###  Exempel

```python

threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
    tc = threadedComments1[i]
    note = tc.notes

```



###  Se även
* modul [aspose.cells](../../)
* klass [CommentCollection](/cells/sv/python-net/aspose.cells/commentcollection)

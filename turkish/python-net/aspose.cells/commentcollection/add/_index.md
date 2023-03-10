---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
Koleksiyona bir yorum ekler.


###  İadeler

[Comment](/cells/tr/python-net/aspose.cells/comment) nesne dizini.


```python
def add(self, cell_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| cell_name | str | Cell adı.|

###  Örnek

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
Koleksiyona bir yorum ekler.


###  İadeler

[Comment](/cells/tr/python-net/aspose.cells/comment) nesne dizini.


```python
def add(self, row, column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row | int | Cell satır dizini.|
| column | int | Cell sütun dizini.|

###  Örnek

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Comment](/cells/tr/python-net/aspose.cells/comment)
* sınıf [CommentCollection](/cells/tr/python-net/aspose.cells/commentcollection)

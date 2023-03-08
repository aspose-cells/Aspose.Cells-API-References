---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/commentcollection/add/
is_root: false
---
##  add(cell_name) {#str}
يضيف تعليقًا إلى المجموعة.


###  عائدات

[Comment](/cells/ar/python-net/aspose.cells/comment) فهرس العنصر.


```python
def add(self, cell_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| cell_name | str | Cell الاسم.|

###  مثال

```python

commentIndex2 = comments.add("B2")
comment2 = comments[commentIndex2]
comment2.note = "Second note."
comment2.font.name = "Times New Roman"

```


##  add(row, column) {#int-int}
يضيف تعليقًا إلى المجموعة.


###  عائدات

[Comment](/cells/ar/python-net/aspose.cells/comment) فهرس العنصر.


```python
def add(self, row, column):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| row | int | Cell فهرس الصف.|
| column | int | Cell فهرس العمود.|

###  مثال

```python

commentIndex1 = comments.add(0, 0)
comment1 = comments[commentIndex1]
comment1.note = "First note."
comment1.font.name = "Times New Roman"

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Comment](/cells/ar/python-net/aspose.cells/comment)
* فئة [CommentCollection](/cells/ar/python-net/aspose.cells/commentcollection)

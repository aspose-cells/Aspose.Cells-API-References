---
title: طريقة get_threaded_comments
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 60
url: /ar/python-net/aspose.cells/commentcollection/get_threaded_comments/
is_root: false
---
##  get_threaded_comments(cell_name) {#str}
يحصل على التعليقات المترابطة حسب اسم الخلية.


###  عائدات




```python
def get_threaded_comments(self, cell_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| cell_name | str | اسم الخلية.|

###  أمثلة

```python

threadedComments2 = comments.get_threaded_comments("B2")
for i in range(len(threadedComments2)):
    tc = threadedComments2[i]
    note = tc.notes

```


##  get_threaded_comments(row, column) {#int-int}
الحصول على التعليقات المترابطة حسب فهرس الصف والعمود.


###  عائدات




```python
def get_threaded_comments(self, row, column):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| row | int | فهرس الصف.|
| column | int | فهرس العمود.|

###  أمثلة

```python

threadedComments1 = comments.get_threaded_comments(1, 1)
for i in range(len(threadedComments1)):
    tc = threadedComments1[i]
    note = tc.notes

```



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [CommentCollection](/cells/ar/python-net/aspose.cells/commentcollection)

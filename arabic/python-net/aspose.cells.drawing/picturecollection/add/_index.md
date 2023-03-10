---
title: طريقة add
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells.drawing/picturecollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, stream):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| stream | io.RawIOBase | كائن دفق يحتوي على بيانات الصورة.|

###  مثال

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs)

```


##  add(upper_left_row, upper_left_column, file_name) {#int-int-str}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, file_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| file_name | str | اسم ملف الصورة.|

###  مثال

```python

# add a picture
pictures.add(1, 1, "image.jpg")

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| lower_right_row | int | فهرس الصف السفلي الأيمن|
| lower_right_column | int | فهرس العمود الأيمن السفلي|
| stream | io.RawIOBase | كائن دفق يحتوي على بيانات الصورة.|

###  مثال

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, 5, 5, fs)

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-str}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| lower_right_row | int | فهرس الصف السفلي الأيمن|
| lower_right_column | int | فهرس العمود الأيمن السفلي|
| file_name | str | اسم ملف الصورة.|

###  مثال

```python

# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")

```


##  add(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| stream | io.RawIOBase | كائن دفق يحتوي على بيانات الصورة.|
| width_scale | int | مقياس عرض الصورة ، نسبة مئوية.|
| height_scale | int | مقياس ارتفاع الصورة ، نسبة مئوية.|

###  مثال

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs, 50, 50)

```


##  add(upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-str-int-int}
يضيف صورة إلى المجموعة.


###  عائدات

[Picture](/cells/ar/python-net/aspose.cells.drawing/picture) فهرس العنصر.


```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| file_name | str | اسم ملف الصورة.|
| width_scale | int | مقياس عرض الصورة ، نسبة مئوية.|
| height_scale | int | مقياس ارتفاع الصورة ، نسبة مئوية.|

###  مثال

```python

# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)
* فئة [PictureCollection](/cells/ar/python-net/aspose.cells.drawing/picturecollection)

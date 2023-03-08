---
title: طريقة replace
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 330
url: /ar/python-net/aspose.cells/workbook/replace/
is_root: false
---
##  replace(place_holder, new_value) {#str-str}
يستبدل قيمة الخلية بسلسلة جديدة.



```python
def replace(self, place_holder, new_value):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_value | str | قيمة السلسلة المطلوب استبدالها|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


##  replace(place_holder, new_value) {#str-int}
يستبدل قيمة الخلية بعدد صحيح جديد.



```python
def replace(self, place_holder, new_value):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_value | int | قيمة عدد صحيح ليحل محلها|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


##  replace(place_holder, new_value) {#str-float}
يستبدل قيمة خلية بمضاعفة جديدة.



```python
def replace(self, place_holder, new_value):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_value | float | قيمة مزدوجة لتحل محلها|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


##  replace(bool_value, new_value) {#bool-any}
يستبدل قيم الخلايا ببيانات جديدة.



```python
def replace(self, bool_value, new_value):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| bool_value | bool | القيمة المنطقية المطلوب استبدالها.|
| new_value | any |قيمة جديدة. يمكن أن تكون سلسلة أو عددًا صحيحًا أو مزدوجًا أو قيمة DateTime.|


##  replace(int_value, new_value) {#int-any}
يستبدل قيم الخلايا ببيانات جديدة.



```python
def replace(self, int_value, new_value):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| int_value | int | قيمة العدد الصحيح المطلوب استبداله.|
| new_value | any |قيمة جديدة. يمكن أن تكون سلسلة أو عددًا صحيحًا أو مزدوجًا أو قيمة DateTime.|


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
يستبدل قيمة الخلية بمصفوفة سلسلة جديدة.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_values | list | مجموعة سلسلة ليحل محلها|
| is_vertical | bool | صحيح - عمودي ، خطأ - أفقي|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
يستبدل قيم الخلايا بمصفوفة عدد صحيح.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_values | list | مجموعة عدد صحيح ليحل محل|
| is_vertical | bool | صحيح - عمودي ، خطأ - أفقي|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
يستبدل قيم الخلايا بمصفوفة مزدوجة.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_values | list | صفيف مزدوج ليحل محل|
| is_vertical | bool | صحيح - عمودي ، خطأ - أفقي|

###  مثال

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_value, options) {#str-str-ReplaceOptions}
يستبدل قيمة الخلية بسلسلة جديدة.



```python
def replace(self, place_holder, new_value, options):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| place_holder | str | Cell نائب|
| new_value | str | قيمة السلسلة المطلوب استبدالها|
| options | [ReplaceOptions](/cells/ar/python-net/aspose.cells/replaceoptions) | خيارات الاستبدال|



###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)

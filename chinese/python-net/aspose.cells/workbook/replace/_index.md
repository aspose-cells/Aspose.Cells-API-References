---
title: replace方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 330
url: /zh/python-net/aspose.cells/workbook/replace/
is_root: false
---
##  replace(place_holder, new_value) {#str-str}
用新字符串替换单元格的值。



```python
def replace(self, place_holder, new_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_value | str |要替换的字符串值|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


##  replace(place_holder, new_value) {#str-int}
用新整数替换单元格的值。



```python
def replace(self, place_holder, new_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_value | int |要替换的整数值|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


##  replace(place_holder, new_value) {#str-float}
用新的双精度替换单元格的值。



```python
def replace(self, place_holder, new_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_value | float |要替换的双值|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


##  replace(bool_value, new_value) {#bool-any}
用新数据替换单元格的值。



```python
def replace(self, bool_value, new_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| bool_value | bool |要替换的布尔值。|
| new_value | any |新价值。可以是字符串、整数、双精度或 DateTime 值。|


##  replace(int_value, new_value) {#int-any}
用新数据替换单元格的值。



```python
def replace(self, int_value, new_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| int_value | int |要替换的整数值。|
| new_value | any |新价值。可以是字符串、整数、双精度或 DateTime 值。|


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
用新的字符串数组替换单元格的值。



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_values | list |要替换的字符串数组|
| is_vertical | bool |真 - 垂直，假 - 水平|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
用整数数组替换单元格的值。



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_values | list |要替换的整数数组|
| is_vertical | bool |真 - 垂直，假 - 水平|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_values, is_vertical) {#str-list-bool}
用双精度数组替换单元格的值。



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_values | list |要替换的双数组|
| is_vertical | bool |真 - 垂直，假 - 水平|

### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


##  replace(place_holder, new_value, options) {#str-str-ReplaceOptions}
用新字符串替换单元格的值。



```python
def replace(self, place_holder, new_value, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| place_holder | str | Cell 占位符|
| new_value | str |要替换的字符串值|
| options | [ReplaceOptions](/cells/zh/python-net/aspose.cells/replaceoptions) |替换选项|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)

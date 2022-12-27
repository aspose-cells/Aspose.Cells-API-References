---
title: get_picture method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 120
url: /python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---

## get_picture(is_header, section) {#bool-int}

Gets the [Picture](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer.

### Returns 


Returns [Picture](/cells/python-net/aspose.cells.drawing/picture) object.
Returns null if there is no picture.


```python
def get_picture(self, is_header, section):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| is_header | bool | Indicates whether it is in the header or footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |


## get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}

Gets the [Picture](/cells/python-net/aspose.cells.drawing/picture) object of the header / footer.

### Returns 


Returns [Picture](/cells/python-net/aspose.cells.drawing/picture) object.


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| is_first | bool | Indicates whether getting the picture of first page header/footer. |
| is_even | bool | Indicates whether getting the picture of even page header/footer. |
| is_header | bool | Indicates whether getting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |



### See Also
* module [aspose.cells](../../)
* class [PageSetup](/cells/python-net/aspose.cells/pagesetup)

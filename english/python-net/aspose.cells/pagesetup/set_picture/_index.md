---
title: set_picture method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 220
url: /python-net/aspose.cells/pagesetup/set_picture/
is_root: false
---

## set_picture(is_first, is_even, is_header, section, image_data) {#bool-bool-bool-int-bytes}

Sets an image in the header/footer of a worksheet.

### Returns 


Returns [Picture](/cells/python-net/aspose.cells.drawing/picture) object.


```python
def set_picture(self, is_first, is_even, is_header, section, image_data):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| is_first | bool | Indicates whether setting the picture of first page header/footer. |
| is_even | bool | Indicates whether setting the picture of even page header/footer. |
| is_header | bool | Indicates whether setting the picture of header/footer. |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| image_data | bytes | Image data. |



### See Also
* module [aspose.cells](../../)
* class [PageSetup](/cells/python-net/aspose.cells/pagesetup)

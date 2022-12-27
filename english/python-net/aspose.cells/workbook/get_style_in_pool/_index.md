---
title: get_style_in_pool method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 190
url: /python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---

## get_style_in_pool(index) {#int}

Gets the style in the style pool.
All styles in the workbook will be gathered into a pool.
There is only a simple reference index in the cells.

### Returns 


The style in the pool corresponds to given index, may be null.


```python
def get_style_in_pool(self, index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| index | int | The index. |
### Remarks

If the returned style is changed, the style of all cells(which refers to this style) will be changed.


### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)

---
title: characters method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 50
url: /python-net/aspose.cells.drawing/lineshape/characters/
is_root: false
---

## characters(start_index, length) {#int-int}

Returns a Characters object that represents a range of characters within the text.

### Returns 


Characters object.


```python
def characters(self, start_index, length):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| start_index | int | The index of the start of the character. |
| length | int | The number of characters. |
### Remarks

This method only works on shape with title.### Example 


`Aspose.Cells.FontSetting fontSetting = shape.Characters(0, 4);`



### See Also
* module [aspose.cells.drawing](../../)
* class [LineShape](/cells/python-net/aspose.cells.drawing/lineshape)

---
title: add_shape_in_chart_by_scale method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 280
url: /python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/
is_root: false
---

## add_shape_in_chart_by_scale(type, placement, left, top, right, bottom) {#MsoDrawingType-PlacementType-float-float-float-float}

Add a shape to chart. All unit is percent scale of chart area.



```python
def add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [MsoDrawingType](/cells/python-net/aspose.cells.drawing/msodrawingtype) | The drawing type. |
| placement | [PlacementType](/cells/python-net/aspose.cells.drawing/placementtype) | the placement type. |
| left | float | Unit is percent scale of chart area width. |
| top | float | Unit is percent scale of chart area height. |
| right | float | Unit is percent scale of chart area width. |
| bottom | float | Unit is percent scale of chart area height. |


## add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data) {#MsoDrawingType-PlacementType-float-float-float-float-bytes}

Add a shape to chart .All unit is 1/4000 of chart area.



```python
def add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom, image_data):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [MsoDrawingType](/cells/python-net/aspose.cells.drawing/msodrawingtype) | The drawing type. |
| placement | [PlacementType](/cells/python-net/aspose.cells.drawing/placementtype) | the placement type. |
| left | float | Unit is percent scale of chart area width. |
| top | float | Unit is percent scale of chart area height. |
| right | float | Unit is percent scale of chart area width. |
| bottom | float | Unit is percent scale of chart area height. |
| image_data | bytes | If the shape is not a picture or ole object,imageData should be null. |



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)

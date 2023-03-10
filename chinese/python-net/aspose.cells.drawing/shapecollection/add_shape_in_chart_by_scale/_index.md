---
title: add_shape_in_chart_by_scale方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 280
url: /zh/python-net/aspose.cells.drawing/shapecollection/add_shape_in_chart_by_scale/
is_root: false
---
##  add_shape_in_chart_by_scale(type, placement, left, top, right, bottom) {#MsoDrawingType-PlacementType-float-float-float-float}
向图表添加形状。所有单位都是图表区域的百分比比例。



```python
def add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/zh/python-net/aspose.cells.drawing/msodrawingtype) |绘图类型。|
| placement | [PlacementType](/cells/zh/python-net/aspose.cells.drawing/placementtype) |展示位置类型。|
| left | float |单位是图表区域宽度的百分比刻度。|
| top | float |单位是图表区域高度的百分比刻度。|
| right | float |单位是图表区域宽度的百分比刻度。|
| bottom | float |单位是图表区域高度的百分比刻度。|


##  add_shape_in_chart_by_scale(type, placement, left, top, right, bottom, image_data) {#MsoDrawingType-PlacementType-float-float-float-float-bytes}
添加图形到图表。所有单位是图表面积的 1/4000。



```python
def add_shape_in_chart_by_scale(self, type, placement, left, top, right, bottom, image_data):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/zh/python-net/aspose.cells.drawing/msodrawingtype) |绘图类型。|
| placement | [PlacementType](/cells/zh/python-net/aspose.cells.drawing/placementtype) |展示位置类型。|
| left | float |单位是图表区域宽度的百分比刻度。|
| top | float |单位是图表区域高度的百分比刻度。|
| right | float |单位是图表区域宽度的百分比刻度。|
| bottom | float |单位是图表区域高度的百分比刻度。|
| image_data | bytes |如果形状不是图片或 ole 对象，imageData 应该为空。|



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ShapeCollection](/cells/zh/python-net/aspose.cells.drawing/shapecollection)

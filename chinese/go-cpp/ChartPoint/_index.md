---
title: "ChartPoint 类"
linktitle: "ChartPoint"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ChartPoint 类。封装在 Go 中表示 chartpoint 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/chartpoint/
---

## ChartPoint class

表示图表中系列的单个点。

```go

type ChartPoint struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetExplosion](./getexplosion/) | 打开的饼块与饼图中心的距离以饼直径的百分比表示。 |
| [SetExplosion](./setexplosion/) | 打开的饼块与饼图中心的距离以饼直径的百分比表示。 |
| [GetShadow](./getshadow/) | 如果 chartpoint 有阴影则为 true。 |
| [SetShadow](./setshadow/) | 如果 chartpoint 有阴影则为 true。 |
| [GetBorder](./getborder/) | 获取 Line</see>。 |
| [GetArea](./getarea/) | 获取 Area</see>。 |
| [GetMarker](./getmarker/) | 获取 Marker。 |
| [GetDataLabels](./getdatalabels/) | 返回一个 DataLabels 对象，表示与此图表点关联的数据标签。 |
| [Get_YValue](./get_yvalue/) | 获取或设置图表点的 Y 值。 |
| [SetYValue](./setyvalue/) | 获取或设置图表点的 Y 值。 |
| [GetYValueType](./getyvaluetype/) | 获取图表点的 Y 值类型。 |
| [GetXValue](./getxvalue/) | 获取或设置图表点的 X 值。 |
| [SetXValue](./setxvalue/) | 获取或设置图表点的 X 值。 |
| [GetXValueType](./getxvaluetype/) | 获取图表点的 X 值类型。 |
| [GetShapeProperties](./getshapeproperties/) | 获取保存 ChartPoint 可视形状属性的 ShapePropertyCollection 对象。 |
| [IsInSecondaryPlot](./isinsecondaryplot/) | 获取或设置一个值，指示此数据点是否位于饼图或条形图的第二个饼或条中。 |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | 获取或设置一个值，指示此数据点是否位于饼图或条形图的第二个饼或条中。 |
| [GetShapeX](./getshapex/) | 在调用 Chart.Calculate() 方法后，获取左上角的 x 坐标，单位为图表宽度的 1/4000。 |
| [GetShapeY](./getshapey/) | 在调用 Chart.Calculate() 方法后，获取左上角的 y 坐标，单位为图表高度的 1/4000。 |
| [GetShapeWidth](./getshapewidth/) | 在调用 Chart.Calculate() 方法后，获取宽度，单位为图表宽度的 1/4000。 |
| [GetShapeHeight](./getshapeheight/) | 在调用 Chart.Calculate() 方法后，获取高度，单位为图表高度的 1/4000。 |
| [GetShapeXPx](./getshapexpx/) | 在调用 Chart.Calculate() 方法后，获取左上角的 x 坐标，单位为像素。 |
| [GetShapeYPx](./getshapeypx/) | 在调用 Chart.Calculate() 方法后，获取左上角的 y 坐标，单位为像素。 |
| [GetShapeWidthPx](./getshapewidthpx/) | 在调用 Chart.Calculate() 方法后，获取宽度，单位为像素。 |
| [GetShapeHeightPx](./getshapeheightpx/) | 在调用 Chart.Calculate() 方法后，获取高度，单位为像素。 |
| [GetBorderWidthPx](./getborderwidthpx/) | 在调用 Chart.Calculate() 方法后，获取边框宽度，单位为像素。 |
| [GetRadiusPx](./getradiuspx/) | 在调用 Chart.Calculate() 方法后，获取气泡、饼图或环形图的半径，单位为像素。 |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | 在调用 Chart.Calculate() 方法后，获取环形图切片的内半径，单位为像素。适用于环形图。 |
| [GetStartAngle](./getstartangle/) | 在调用 Chart.Calculate() 方法后，获取饼图部分的起始角度，以 x 轴顺时针方向度数计量。适用于饼图。 |
| [GetEndAngle](./getendangle/) | 在调用 Chart.Calculate() 方法后，获取饼图部分的结束角度，以 x 轴顺时针方向度数计量。适用于饼图。 |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 x 坐标。适用于饼图和环形图。 |
| [GetArcStartPointYPx](./getarcstartpointypx/) | 在调用 Chart.Calculate() 方法后，获取饼图部分起始点的 y 坐标。适用于饼图和环形图。 |
| [GetArcEndPointXPx](./getarcendpointxpx/) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 x 坐标。适用于饼图和环形图。 |
| [GetArcEndPointYPx](./getarcendpointypx/) | 在调用 Chart.Calculate() 方法后，获取饼图部分结束点的 y 坐标。适用于饼图和环形图。 |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | 在调用 Chart.Calculate() 方法后，获取环形图部分起始点的 x 坐标。适用于环形图。 |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | 在调用 Chart.Calculate() 方法后，获取环形图部分起始点的 y 坐标。适用于环形图。 |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | 获取在调用 Chart.Calculate() 方法后饼图部分结束点的 x 坐标。适用于环形图。 |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | 获取在调用 Chart.Calculate() 方法后饼图部分结束点的 y 坐标。适用于环形图。 |
| [GetTopPointCount](./gettoppointcount/) | 获取在调用 Chart.Calculate() 方法后顶部点的数量。 |
| [GetTopPointXPx](./gettoppointxpx/) | 获取在调用 Chart.Calculate() 方法后形状顶部点的 x 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D。 |
| [GetTopPointYPx](./gettoppointypx/) | 获取在调用 Chart.Calculate() 方法后形状顶部点的 y 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D。 |
| [GetBottomPointCount](./getbottompointcount/) | 获取在调用 Chart.Calculate() 方法后底部点的数量。 |
| [GetBottomPointXPx](./getbottompointxpx/) | 获取在调用 Chart.Calculate() 方法后形状底部点的 x 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid。 |
| [GetBottomPointYPx](./getbottompointypx/) | 获取在调用 Chart.Calculate() 方法后形状底部点的 y 坐标。适用于 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid。 |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | 获取在调用 Chart.Calculate() 方法后类别轴上点的数量。仅适用于面积图。 |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | 获取在调用 Chart.Calculate() 方法后类别轴上点的 x 坐标。仅适用于面积图。 |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | 获取在调用 Chart.Calculate() 方法后类别轴上点的 y 坐标。仅适用于面积图。 |

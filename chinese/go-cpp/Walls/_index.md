---
title: "Walls 类"
linktitle: "Walls"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Walls 类。封装表示 Go 中墙体的对象。"
type: docs
weight: 200
url: /zh/go-cpp/walls/
---

## Walls class

封装表示三维图表墙面的对象。

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewWalls](./newwalls/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCenterX](./getcenterx/) | 在调用 Chart.Calculate() 方法后，获取墙体中心左下角的 x 坐标，单位为图表宽度的 1/4000。 |
| [GetCenterY](./getcentery/) | 在调用 Chart.Calculate() 方法后，获取墙体中心左下角的 y 坐标，单位为图表高度的 1/4000。 |
| [GetWidth](./getwidth/) | 在调用 Chart.Calculate() 方法后，获取从左到右的宽度，单位为图表宽度的 1/4000。 |
| [GetDepth](./getdepth/) | 在调用 Chart.Calculate() 方法后，获取从前到后的深度，单位为图表宽度的 1/4000。 |
| [GetHeight](./getheight/) | 在调用 Chart.Calculate() 方法后，获取从上到下的高度，单位为图表高度的 1/4000。 |
| [GetCenterXPx](./getcenterxpx/) | 在调用 Chart.Calculate() 方法后，获取墙体中心左下角的 x 坐标，单位为像素。 |
| [GetCenterYPx](./getcenterypx/) | 在调用 Chart.Calculate() 方法后，获取墙体中心左下角的 y 坐标，单位为像素。 |
| [GetWidthPx](./getwidthpx/) | 在调用 Chart.Calculate() 方法后，获取从左到右的宽度，单位为像素。 |
| [GetDepthPx](./getdepthpx/) | 在调用 Chart.Calculate() 方法后，获取从前到后的深度，单位为像素。 |
| [GetHeightPx](./getheightpx/) | 在调用 Chart.Calculate() 方法后，以像素为单位获取从上到下的高度。 |
| [GetCubePointCount](./getcubepointcount/) | 在调用 Chart.Calculate() 方法后获取立方体点的数量。 |
| [GetCubePointXPx](./getcubepointxpx/) | 在调用 Chart.Calculate() 方法后获取墙体立方体顶点的 X 坐标。墙体立方体的顶点数量为八个。 |
| [GetCubePointYPx](./getcubepointypx/) | 在调用 Chart.Calculate() 方法后获取墙体立方体顶点的 Y 坐标。墙体立方体的顶点数量为八个。 |
| [GetBackgroundColor](./getbackgroundcolor/) | 获取或设置区域的背景颜色。 |
| [SetBackgroundColor](./setbackgroundcolor/) | 获取或设置区域的背景颜色。 |
| [GetForegroundColor](./getforegroundcolor/) | 获取或设置前景颜色。 |
| [SetForegroundColor](./setforegroundcolor/) | 获取或设置前景颜色。 |
| [GetFormatting](./getformatting/) | 表示区域的格式设置。 |
| [SetFormatting](./setformatting/) | 表示区域的格式设置。 |
| [GetInvertIfNegative](./getinvertifnegative/) | 如果属性为 true 且图表点的值为负数，前景颜色和背景颜色将互换。 |
| [SetInvertIfNegative](./setinvertifnegative/) | 如果属性为 true 且图表点的值为负数，前景颜色和背景颜色将互换。 |
| [GetFillFormat](./getfillformat/) | 表示一个 FillFormat 对象，其中包含指定图表或形状的填充格式属性。 |
| [GetTransparency](./gettransparency/) | 返回或设置该区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [SetTransparency](./settransparency/) | 返回或设置该区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [GetBorder](./getborder/) | 获取或设置边框线。 |
| [SetBorder](./setborder/) | 获取或设置边框线。 |

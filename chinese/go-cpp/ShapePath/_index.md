---
title: "ShapePath 类"
linktitle: "ShapePath"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ShapePath 类。封装在 Go 中表示 shapepath 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shapepath/
---

## ShapePath class

表示由一系列移动、直线和曲线组成的创建路径，组合后形成几何形状。

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewShapePath](./newshapepath/) | 初始化 ShapePath 类的新实例。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetPathSegments](./getpathsegments/) | 获取 ShapeSegmentPathCollection 列表 |
| [GetWidthPixel](./getwidthpixel/) | 获取此路径的宽度（单位：像素）。 |
| [SetWidthPixel](./setwidthpixel/) | 获取此路径的宽度（单位：像素）。 |
| [GetHeightPixel](./getheightpixel/) | 获取此路径的高度（单位：像素）。 |
| [SetHeightPixel](./setheightpixel/) | 获取此路径的高度（单位：像素）。 |
| [MoveTo](./moveto/) | 从指定点开始新图形而不关闭当前图形。随后添加到路径的所有点都将添加到此新图形。单位：像素。 |
| [LineTo](./lineto/) | 向当前图形追加线段。起始点为当前图形的终点。单位：像素。 |
| [CubicBezierTo](./cubicbezierto/) | 向当前图形追加三次贝塞尔曲线。起始点为当前图形的终点。单位：像素。 |
| [ArcTo](./arcto/) | 向当前图形追加椭圆弧。起始点为当前图形的终点。 |
| [Close](./close/) | 关闭当前图形并开始新图形。如果当前图形包含一系列相连的线段和曲线，方法将通过从终点连接到起点的线段来闭合环路。 |

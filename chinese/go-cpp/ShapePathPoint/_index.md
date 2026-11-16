---
title: "ShapePathPoint 类"
linktitle: "ShapePathPoint"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ShapePathPoint 类。封装在 Go 中表示 shapepathpoint 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shapepathpoint/
---

## ShapePathPoint class

指定位置坐标或角度标记。位置坐标表示路径在坐标空间中的坐标（例如 X/Y）。角度标记指示路径中的角度变化（例如弧线的起始角度和摆幅角度）。

```go

type ShapePathPoint struct  {
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
| [GetXPixel](./getxpixel/) | 当对象是位置坐标时，获取或设置以像素为单位的 x 坐标。 |
| [SetXPixel](./setxpixel/) | 当对象是位置坐标时，获取或设置以像素为单位的 x 坐标。 |
| [GetYPixel](./getypixel/) | 当对象是位置坐标时，获取或设置以像素为单位的 y 坐标。 |
| [SetYPixel](./setypixel/) | 当对象是位置坐标时，获取或设置以像素为单位的 y 坐标。 |
| [GetXAngle](./getxangle/) | 当对象是角度标记时，获取或设置第一角度（单位为度）。 |
| [SetXAngle](./setxangle/) | 当对象是角度标记时，获取或设置第一角度（单位为度）。 |
| [GetYAngle](./getyangle/) | 当对象是角度标记时，获取或设置第二角度（单位为度）。 |
| [SetYAngle](./setyangle/) | 当对象是角度标记时，获取或设置第二角度（单位为度）。 |
| [GetType](./gettype/) | 指定当前对象的值类型。 |

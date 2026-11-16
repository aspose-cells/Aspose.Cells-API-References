---
title: "ShapePathType 枚举"
linktitle: "ShapePathType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ShapePathType 枚举。封装在 Go 中表示 shapepathtype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/shapepathtype/
---

## ShapePathType Enum

表示路径段类型。

```go

type ShapePathType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [LineTo](./lineto/) | 直线段 |
| [CubicBezierCurveTo](./cubicbeziercurveto/) | 三次贝塞尔曲线 |
| [MoveTo](./moveto/) | 开始新路径 |
| [Close](./close/) | 如果起始 POINT 和结束 POINT 不相同，则绘制一条单直线将路径的起始 POINT 与结束 POINT 连接起来。 |
| [End](./end/) | 当前路径的结束 |
| [Escape](./escape/) | 退出 |
| [ArcTo](./arcto/) | 弧线 |
| [Unknown](./unknown/) | 未知 |

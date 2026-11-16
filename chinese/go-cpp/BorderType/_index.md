---
title: "BorderType 枚举"
linktitle: "BorderType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "BorderType 枚举。封装在 Go 中表示 bordertype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/bordertype/
---

## BorderType Enum

枚举边框线和对角线类型。

```go

type BorderType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [LeftBorder](./leftborder/) | 表示左边框线。 |
| [RightBorder](./rightborder/) | 表示右边框线存在。 |
| [TopBorder](./topborder/) | 表示上边框线。 |
| [BottomBorder](./bottomborder/) | 表示下边框线。 |
| [DiagonalDown](./diagonaldown/) | 表示从左上到右下的对角线。 |
| [DiagonalUp](./diagonalup/) | 表示从左下到右上的对角线。 |
| [Vertical](./vertical/) | 仅适用于动态样式，例如条件格式、数据透视表。 |
| [Horizontal](./horizontal/) | 仅适用于动态样式，例如条件格式、数据透视表。 |
| [SideBorders](./sideborders/) | 指示四个侧边框：<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> 和 <see cref="BottomBorder"/>。 |
| [Diagonal](./diagonal/) | 为某些 API 的用户便利提供的多边框特殊组合。指示 <see cref="DiagonalUp"/> 和 <see cref="DiagonalDown"/> 的对角线边框。 |
| [DynamicStyleBorders](./dynamicstyleborders/) | 指示动态样式的 <see cref="Vertical"/> 和 <see cref="Horizontal"/>。 |
| [None](./none/) | 未指定任何边框。 |

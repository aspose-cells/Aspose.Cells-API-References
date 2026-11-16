---
title: "CellsColor 类"
linktitle: "CellsColor"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellsColor 类。封装在 Go 中表示 cellscolor 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cellscolor/
---

## CellsColor class

表示所有颜色类型。

```go

type CellsColor struct  {
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
| [IsShapeColor](./isshapecolor/) | 获取并设置应应用于单元格或形状的颜色。 |
| [SetIsShapeColor](./setisshapecolor/) | 获取并设置应应用于单元格或形状的颜色。 |
| [GetType](./gettype/) | 颜色类型。 |
| [GetThemeColor](./getthemecolor/) | 获取主题颜色。仅适用于主题颜色类型。 |
| [SetThemeColor](./setthemecolor/) | 获取主题颜色。仅适用于主题颜色类型。 |
| [GetColorIndex](./getcolorindex/) | 获取并设置颜色调色板中的颜色索引。仅适用于索引颜色。 |
| [SetColorIndex](./setcolorindex/) | 获取并设置颜色调色板中的颜色索引。仅适用于索引颜色。 |
| [GetColor](./getcolor/) | 获取并设置 RGB 颜色。 |
| [SetColor](./setcolor/) | 获取并设置 RGB 颜色。 |
| [GetArgb](./getargb/) | 获取并设置来自 32 位 ARGB 值的颜色。 |
| [SetArgb](./setargb/) | 获取并设置来自 32 位 ARGB 值的颜色。 |
| [GetTransparency](./gettransparency/) | 获取并设置透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [SetTransparency](./settransparency/) | 获取并设置透明度，取值范围为 0.0（不透明）到 1.0（透明）。 |
| [SetTintOfShapeColor](./settintofshapecolor/) | 设置形状颜色的色调 |

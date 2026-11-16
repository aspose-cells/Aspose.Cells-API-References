---
title: "DefaultStyleSettings 类"
linktitle: "DefaultStyleSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DefaultStyleSettings 类。封装了在 Go 中表示 defaultstylesettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/defaultstylesettings/
---

## DefaultStyleSettings class

工作簿样式属性默认值的设置。

```go

type DefaultStyleSettings struct  {
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
| [GetBuiltInPreference](./getbuiltinpreference/) | 指示当样式同时定义了内置数字和自定义模式时，是否更倾向于使用数字格式属性。默认值为 false，这意味着默认情况下只要自定义模式非空，就会使用自定义模式来格式化值。 |
| [SetBuiltInPreference](./setbuiltinpreference/) | 指示当样式同时定义了内置数字和自定义模式时，是否更倾向于使用数字格式属性。默认值为 false，这意味着默认情况下只要自定义模式非空，就会使用自定义模式来格式化值。 |
| [GetFontName](./getfontname/) | 获取/设置工作簿的默认字体名称 |
| [SetFontName](./setfontname/) | 获取/设置工作簿的默认字体名称 |
| [GetFontSize](./getfontsize/) | 获取/设置工作簿的默认标准字体大小。 |
| [SetFontSize](./setfontsize/) | 获取/设置工作簿的默认标准字体大小。 |
| [GetHorizontalAlignment](./gethorizontalalignment/) | 获取/设置水平对齐的默认值 |
| [SetHorizontalAlignment](./sethorizontalalignment/) | 获取/设置水平对齐的默认值 |
| [GetVerticalAlignment](./getverticalalignment/) | 获取/设置垂直对齐的默认值 |
| [SetVerticalAlignment](./setverticalalignment/) | 获取/设置垂直对齐的默认值 |

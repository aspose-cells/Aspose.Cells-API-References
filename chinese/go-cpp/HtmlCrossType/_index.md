---
title: "HtmlCrossType 枚举"
linktitle: "HtmlCrossType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "HtmlCrossType 枚举。封装在 Go 中表示 htmlcrosstype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

表示五种 HTML 交叉字符串类型。

```go

type HtmlCrossType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Default](./default/) | 显示方式类似 MS Excel，取决于下一个单元格。如果下一个单元格为 null，字符串将跨越，否则将被截断。 |
| [MSExport](./msexport/) | 显示字符串的方式类似 MS Excel 导出 HTML。 |
| [Cross](./cross/) | 显示 HTML 交叉字符串，此创建大型 HTML 文件的性能将比将值设置为 Default 或 FitToCell 快十倍以上。 |
| [CrossHideRight](./crosshideright/) | 显示 HTML 交叉字符串，并在文本重叠时隐藏右侧字符串。 |
| [FitToCell](./fittocell/) | 仅在单元格宽度范围内显示字符串。 |

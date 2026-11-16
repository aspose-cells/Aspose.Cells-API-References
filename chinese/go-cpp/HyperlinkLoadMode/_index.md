---
title: "HyperlinkLoadMode 枚举"
linktitle: "HyperlinkLoadMode"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "HyperlinkLoadMode 枚举。封装在 Go 中表示 hyperlinkloadmode 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

指定加载 HTML 时超链接的处理方式。

```go

type HyperlinkLoadMode int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Normal](./normal/) | 仅加载单元格中的第一个超链接，后续的将被忽略。 |
| [AllowMultiple](./allowmultiple/) | 单元格中的所有超链接都会添加到 <see cref="Worksheet.Hyperlinks"/>。请注意，MS Excel 本身每个单元格仅支持一个超链接，因此此选项可能生成 Excel 无法完全呈现的文件。 |

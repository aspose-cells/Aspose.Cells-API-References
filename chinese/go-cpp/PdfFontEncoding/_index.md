---
title: "PdfFontEncoding 枚举"
linktitle: "PdfFontEncoding"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PdfFontEncoding 枚举。封装在 Go 中表示 pdffontencoding 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pdffontencoding/
---

## PdfFontEncoding Enum

表示 PDF 嵌入字体的编码。

```go

type PdfFontEncoding int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Identity](./identity/) | 表示在 pdf 中对所有嵌入字体使用 Identity-H 编码。 |
| [AnsiPrefer](./ansiprefer/) | 表示倾向于对字符范围 32-127 的 TrueType 字体使用 WinAnsiEncoding，否则将在 pdf 中对嵌入字体使用 Identity-H 编码。 |

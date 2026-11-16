---
title: "TxtValueQuoteType 枚举"
linktitle: "TxtValueQuoteType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TxtValueQuoteType 枚举。封装在 Go 中表示 txtvaluequotetype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

指定在文本格式文件中为值使用引号的类型。

```go

type TxtValueQuoteType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Normal](./normal/) | 所有包含特殊字符（如引号、分隔符）的值都会被加引号。行为与 Microsoft Excel 导出文本文件时相同。 |
| [Always](./always/) | 所有值始终会被加引号。 |
| [Minimum](./minimum/) | 仅在需要时对值加引号。例如，如果一个值包含引号但引号不在该值的开头，则该值不会加引号。 |
| [Never](./never/) | 所有值都不会加引号。使用此类型导出的文本文件可能无法正确读取，因为缺少必要的引号。 |

---
title: "CellValueType 枚举"
linktitle: "CellValueType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellValueType 枚举。封装在 Go 中表示 cellvaluetype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cellvaluetype/
---

## CellValueType Enum

指定单元格值的类型。

```go

type CellValueType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [IsUnknown](./isunknown/) | 单元格值类型未知。 |
| [IsNull](./isnull/) | 空白单元格。对应的值应为 null。 |
| [IsNumeric](./isnumeric/) | 单元格值为数值。对应的值必须是 int 或 double。 |
| [IsDateTime](./isdatetime/) | 单元格值为日期时间。对应的值必须是 DateTime。 |
| [IsString](./isstring/) | 单元格值为字符串。对应的值必须是 string。 |
| [IsBool](./isbool/) | 单元格值为布尔值。对应的值必须是 bool。 |
| [IsError](./iserror/) | 单元格包含错误值。相应的值必须是错误字符串。 |

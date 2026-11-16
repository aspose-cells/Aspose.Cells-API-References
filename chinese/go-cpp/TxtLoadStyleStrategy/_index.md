---
title: "TxtLoadStyleStrategy 枚举"
linktitle: "TxtLoadStyleStrategy"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TxtLoadStyleStrategy 枚举。封装表示 Go 中 txtloadstylestrategy 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/txtloadstylestrategy/
---

## TxtLoadStyleStrategy Enum

指定在将字符串值转换为数字或日期时间时，如何为解析后的值应用样式。

```go

type TxtLoadStyleStrategy int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [None](./none/) | 不为解析值设置样式。 |
| [BuiltIn](./builtin/) | 当解析值为普通数字/日期时间值时，将样式设置为内置的数字/日期时间格式。 |
| [ExactFormat](./exactformat/) | 为解析值设置精确的自定义格式，使格式化后的值与原始输入保持一致。 |

---
title: "ControlMatchEntryType 枚举"
linktitle: "ControlMatchEntryType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ControlMatchEntryType 枚举。封装了在 Go 中表示 controlmatchentrytype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/controlmatchentrytype/
---

## ControlMatchEntryType Enum

表示 ListBox 或 ComboBox 在用户输入时如何搜索其列表。

```go

type ControlMatchEntryType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [FirstLetter](./firstletter/) | 该控件搜索以输入字符开头的下一个条目。重复输入相同的字母会循环遍历所有以该字母开头的条目。 |
| [Complete](./complete/) | 当每个字符被输入时，控件会搜索匹配所有已输入字符的条目。 |
| [None](./none/) | 当输入字符时，列表不会被搜索。 |

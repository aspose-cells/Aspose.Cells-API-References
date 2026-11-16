---
title: "Date 结构体"
linktitle: "日期"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Date 结构体。封装在 Go 中表示日期的对象。"
type: docs
weight: 200
url: /zh/go-cpp/date/
---

## Date Struct

表示日期和时间。

```go

type Date int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [year](./year/) | 年份组件（1-9999）。 |
| [month](./month/) | 月份组件（1-12）。 |
| [day](./day/) | 日期组件（1-31）。 |
| [hour](./hour/) | 小时组件（0-23）。 |
| [minute](./minute/) | 分钟组件（0-59）。 |
| [second](./second/) | 秒组件（0-59）。 |
| [millisecond](./millisecond/) | 毫秒组件（0-999）。 |
| [dateKind](./datekind/) | 指定时间是本地时间、UTC 还是未指定。默认值为未指定。 |

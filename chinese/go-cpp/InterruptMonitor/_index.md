---
title: "InterruptMonitor 类"
linktitle: "InterruptMonitor"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "InterruptMonitor 类。封装在 Go 中表示 interruptmonitor 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/interruptmonitor/
---

## InterruptMonitor class

表示关于中断的所有操作符。

```go

type InterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewInterruptMonitor](./newinterruptmonitor/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsInterruptionRequested](./isinterruptionrequested/) | 将监视器标记为请求中断 |
| [Interrupt](./interrupt/) | 中断当前操作员。 |

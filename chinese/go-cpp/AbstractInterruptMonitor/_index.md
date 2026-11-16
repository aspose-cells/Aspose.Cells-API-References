---
title: "AbstractInterruptMonitor 类"
linktitle: "AbstractInterruptMonitor"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AbstractInterruptMonitor 类。封装在 Go 中表示 abstractinterruptmonitor 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

监视所有耗时操作中的中断请求。

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | 当过程被中断时，是否安静地终止过程或抛出异常。默认值为 false，即当 IsInterruptionRequested 为 true 时，将抛出代码为 ExceptionType.Interrupted 的 CellsException。 |

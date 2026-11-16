---
title: "GetTerminateWithoutException 方法"
linktitle: "GetTerminateWithoutException"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetTerminateWithoutException 方法。封装了在 Go 中表示 getterminatewithoutexception 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/abstractinterruptmonitor/getterminatewithoutexception/
---

## GetTerminateWithoutException function

当过程被中断时，是否安静地终止过程或抛出异常。默认值为 false，即当 IsInterruptionRequested 为 true 时，将抛出代码为 ExceptionType.Interrupted 的 CellsException。

```go

func (instance *AbstractInterruptMonitor) GetTerminateWithoutException()  (bool,  error) 

```

## 备注


## 另请参阅

* Class [AbstractInterruptMonitor](../)
* Library [Aspose.Cells for Go](../../)

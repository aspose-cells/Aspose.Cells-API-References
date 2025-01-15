---
title: AbstractInterruptMonitor Class 
linktitle: AbstractInterruptMonitor
second_title: Aspose.Cells for Go via C++ API Reference
description: 'AbstractInterruptMonitor class. Encapsulates the object that represents abstractinterruptmonitor in Go.'
type: docs
weight: 200
url: /go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[GetTerminateWithoutException](./getterminatewithoutexception/) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.Default is false, that is, when IsInterruptionRequested is true,a CellsException with code ExceptionType.Interrupted will be thrown. | 

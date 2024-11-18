---
title: AbstractInterruptMonitor Class 
linktitle: AbstractInterruptMonitor
second_title: Aspose.Cells for Go API Reference
description: 'AbstractInterruptMonitor class. Encapsulates the object that represents abstractinterruptmonitor in Go.'
type: docs
weight: 200
url: /go/aspose.cells/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

```go

type AbstractInterruptMonitor struct 

abstractinterruptmonitor, _ := asposecells.NewAbstractInterruptMonitor()

```

## Methods

| Method | Description |
| --- | --- |
|[GetTerminateWithoutException](./getterminatewithoutexception/) | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.Default is false, that is, when <see cref="IsInterruptionRequested"/> is true,a <see cref="CellsException"/> with code <see cref="ExceptionType.Interrupted"/> will be thrown. | 

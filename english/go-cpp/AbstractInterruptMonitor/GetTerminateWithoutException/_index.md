---
title: GetTerminateWithoutException Method 
linktitle: GetTerminateWithoutException
second_title: Aspose.Cells for Go API Reference
description: 'GetTerminateWithoutException method. Encapsulates the function that represents getterminatewithoutexception in Go.'
type: docs
weight: 200
url: /go-cpp/abstractinterruptmonitor/getterminatewithoutexception/
---

## GetTerminateWithoutException function

When procedure is interrupted, whether terminate the procedure quietly or throw an Exception.Default is false, that is, when <see cref="IsInterruptionRequested"/> is true,a <see cref="CellsException"/> with code <see cref="ExceptionType.Interrupted"/> will be thrown.

```go

func (instance *AbstractInterruptMonitor) GetTerminateWithoutException()  (bool,  error) 

```

## Remarks


## See Also

* Class [AbstractInterruptMonitor](../)
* Namespace [Aspose.Cells](../../)
* Library [Aspose.Cells for Go](../../../)

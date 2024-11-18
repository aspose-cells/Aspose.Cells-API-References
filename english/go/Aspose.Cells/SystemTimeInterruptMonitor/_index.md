---
title: SystemTimeInterruptMonitor Class 
linktitle: SystemTimeInterruptMonitor
second_title: Aspose.Cells for Go API Reference
description: 'SystemTimeInterruptMonitor class. Encapsulates the object that represents systemtimeinterruptmonitor in Go.'
type: docs
weight: 200
url: /go/aspose.cells/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Simple implementation of <see cref="AbstractInterruptMonitor"/> by checking and comparing current system time with user specified limit.

```go

type SystemTimeInterruptMonitor struct 

systemtimeinterruptmonitor, _ := asposecells.NewSystemTimeInterruptMonitor()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[StartMonitor](./startmonitor/) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called,so the procedure which needs to be monitored should be started just after this call. | 
|[IsInterruptionRequested](./isinterruptionrequested/) | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. | 
|[GetTerminateWithoutException](./getterminatewithoutexception/) | See <see cref="AbstractInterruptMonitor.TerminateWithoutException"/>.This property is specified by user when constructing this monitor instance. | 

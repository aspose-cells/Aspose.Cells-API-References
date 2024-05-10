---
title: Class ThreadInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadInterruptMonitor class. Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit
type: docs
url: /net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Simple implementation of [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) by starting another thread to require the interruption after sleeping user specified limit.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Constructors

| Name | Description |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Constructs one interruption monitor. |

## Properties

| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | See [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |

## Methods

| Name | Description |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Finishes the monitor for one procedure. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |

### Remarks

One monitor instance can be used repeatedly, as long as you monitor each process in sequence. It should not be used to monitor multiple procedures concurrently in multi-threads.

### Examples

The following example shows how to monitor the load and save procedure with specified time limit:

```csharp
[C#]

ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
monitor.StartMonitor(1000); //time limit is 1 second
Workbook wb = new Workbook("Large.xlsx", lopts);
//if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
//otherwise finishes the monitor thread and starts to monitor the save procedure
monitor.FinishMonitor();
monitor.StartMonitor(1500); //time limit is 1.5 seconds
wb.Save("result.xlsx");
monitor.FinishMonitor();
```

### See Also

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



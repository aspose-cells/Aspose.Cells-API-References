---
title: Class SystemTimeInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SystemTimeInterruptMonitor class. Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit
type: docs
url: /net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Simple implementation of [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) by checking and comparing current system time with user specified limit.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Constructors

| Name | Description |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Constructs one interruption monitor. |

## Properties

| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | See [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |

## Methods

| Name | Description |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |

### Remarks

This implementation is just a simple solution for simple scenarios. It needs to frequently retrieve and check the system time so itself may have a negative impact on performance to some extent.

### Examples

The following example shows how to monitor the load and save procedure with specified time limit:

```csharp
[C#]

SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
monitor.StartMonitor(1000); //time limit is 1 second
Workbook wb = new Workbook("Large.xlsx", lopts);
//if the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
//otherwise starts to monitor the save procedure
monitor.StartMonitor(1500); //time limit is 1.5 seconds
wb.Save("result.xlsx");
```

### See Also

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: Class AbstractInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractInterruptMonitor class. Monitor for interruption requests in all timeconsuming operations
type: docs
url: /net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

```csharp
public abstract class AbstractInterruptMonitor
```

## Properties

| Name | Description |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [`IsInterruptionRequested`](./isinterruptionrequested/) is true, a [`CellsException`](../cellsexception/) with code Interrupted will be thrown. |

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



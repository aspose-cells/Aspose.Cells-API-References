---
title: ThreadInterruptMonitor.FinishMonitor
second_title: Aspose.Cells for .NET API Reference
description: ThreadInterruptMonitor method. Finishes the monitor for one procedure
type: docs
url: /net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Finishes the monitor for one procedure.

```csharp
public void FinishMonitor()
```

### Remarks

Calling this method after the monitored procedure can release the monitor thread earlier, especially when there is no interruption for it(the time cost of that procedure is less than the specified time limit).

### See Also

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



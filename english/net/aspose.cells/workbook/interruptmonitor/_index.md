---
title: Workbook.InterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the interrupt monitor
type: docs
url: /net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Gets and sets the interrupt monitor.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Examples

```csharp
// Called: wb.InterruptMonitor = new TimeInterruptMonitor(msTimeLimit, msgHeader, msTimeDelay);
public static void Property_InterruptMonitor(Workbook wb, int msTimeLimit, string msgHeader, int[] msTimeDelay)
        {
            wb.InterruptMonitor = new TimeInterruptMonitor(msTimeLimit, msgHeader, msTimeDelay);
            if (msgHeader != null)
            {
                Console.WriteLine(msgHeader + &quot;: starting...&quot;);
            }
        }
```

### See Also

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



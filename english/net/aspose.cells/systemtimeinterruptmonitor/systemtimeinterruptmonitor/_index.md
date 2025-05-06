---
title: SystemTimeInterruptMonitor.SystemTimeInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: SystemTimeInterruptMonitor constructor. Constructs one interruption monitor
type: docs
url: /net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Constructs one interruption monitor.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Examples

```csharp
// Called: SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
public static void SystemTimeInterruptMonitor_Constructor()
        {
            // Create an instance of SystemTimeInterruptMonitor with terminateWithoutException set to false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Create LoadOptions and set the InterruptMonitor to the created monitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Start monitoring with a time limit of 1000 milliseconds (1 second)
            monitor.StartMonitor(1000);

            try
            {
                // Load a workbook with the specified LoadOptions
                Workbook wb = new Workbook(&quot;Large.xlsx&quot;, lopts);

                // If the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
                // Otherwise, start to monitor the save procedure with a new time limit
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Save the workbook
                wb.Save(&quot;SystemTimeInterruptMonitorExample.xlsx&quot;);
            }
            catch (Exception ex)
            {
                Console.WriteLine(&quot;Operation interrupted: &quot; + ex.Message);
            }
        }
```

### See Also

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



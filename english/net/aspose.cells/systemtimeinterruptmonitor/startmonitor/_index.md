---
title: SystemTimeInterruptMonitor.StartMonitor
second_title: Aspose.Cells for .NET API Reference
description: SystemTimeInterruptMonitor method. Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called so the procedure which needs to be monitored should be started just after this call
type: docs
url: /net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

```csharp
public void StartMonitor(int msLimit)
```

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Int32 | time limit(ms) to require the interruption. |

### Examples

```csharp
// Called: monitor.StartMonitor(1000);
public static void Method_Int32_()
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
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // If the time cost of loading the template file exceeds one second, interruption will be required and exception will be thrown here
                // Otherwise, start to monitor the save procedure with a new time limit
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Save the workbook
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
```

### See Also

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



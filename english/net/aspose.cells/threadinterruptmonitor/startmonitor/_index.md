---
title: ThreadInterruptMonitor.StartMonitor
second_title: Aspose.Cells for .NET API Reference
description: ThreadInterruptMonitor method. Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called so the procedure which needs to be monitored should be started just after this call
type: docs
url: /net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

```csharp
public void StartMonitor(int msLimit)
```

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Int32 | time limit(ms) to require the interruption. |

### Examples

```csharp
// Called: monitor.StartMonitor(1500);
public static void Method_Int32_()
        {
            // Create an instance of ThreadInterruptMonitor with terminateWithoutException set to false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Create LoadOptions and set the InterruptMonitor to the created monitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Start the monitor with a time limit of 1000 milliseconds (1 second)
            monitor.StartMonitor(1000);

            try
            {
                // Load a workbook with the specified LoadOptions
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Finish the monitor for the loading procedure
                monitor.FinishMonitor();

                // Start the monitor again with a new time limit of 1500 milliseconds (1.5 seconds)
                monitor.StartMonitor(1500);

                // Save the workbook
                wb.Save("result.xlsx");

                // Finish the monitor for the saving procedure
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
```

### See Also

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



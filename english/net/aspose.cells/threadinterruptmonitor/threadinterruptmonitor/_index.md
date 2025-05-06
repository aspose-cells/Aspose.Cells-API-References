---
title: ThreadInterruptMonitor.ThreadInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: ThreadInterruptMonitor constructor. Constructs one interruption monitor
type: docs
url: /net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Constructs one interruption monitor.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Examples

```csharp
// Called: ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
public static void ThreadInterruptMonitor_Constructor()
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
                Workbook wb = new Workbook(&quot;Large.xlsx&quot;, lopts);

                // Finish the monitor for the loading procedure
                monitor.FinishMonitor();

                // Start the monitor again with a new time limit of 1500 milliseconds (1.5 seconds)
                monitor.StartMonitor(1500);

                // Save the workbook
                wb.Save(&quot;result.xlsx&quot;);

                // Finish the monitor for the saving procedure
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine(&quot;An exception occurred: &quot; + ex.Message);
            }
        }
```

### See Also

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



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

### Examples

```csharp
// Called: monitor.FinishMonitor();
public static void Method_FinishMonitor()
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



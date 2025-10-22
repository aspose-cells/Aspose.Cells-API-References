##ThreadInterruptMonitor.FinishMonitor
ThreadInterruptMonitor method. Finishes the monitor for one procedure
## ThreadInterruptMonitor.FinishMonitor method
Finishes the monitor for one procedure.
```csharp
public void FinishMonitor()
```
### Remarks
Calling this method after the monitored procedure can release the monitor thread earlier, especially when there is no interruption for it(the time cost of that procedure is less than the specified time limit).
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadInterruptMonitorMethodFinishMonitorDemo
{
public static void Run()
{
// Create an instance of ThreadInterruptMonitor
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
// Create LoadOptions and set the InterruptMonitor
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
// Start monitoring with 1 second timeout
monitor.StartMonitor(1000);
try
{
// Simulate a long-running operation
for (int i = 0; i < 5; i++)
{
System.Threading.Thread.Sleep(200);
Console.WriteLine($"Processing step {i + 1}");
}
// Finish monitoring the operation
monitor.FinishMonitor();
Console.WriteLine("Operation completed successfully");
}
catch (Exception ex)
{
Console.WriteLine("An exception occurred: " + ex.Message);
}
}
}
}
```
### See Also
* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

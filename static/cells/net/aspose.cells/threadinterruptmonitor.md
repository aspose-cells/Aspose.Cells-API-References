##Class ThreadInterruptMonitor
Aspose.Cells.ThreadInterruptMonitor class. Simple implementation of AbstractInterruptMonitor by starting another thread to require the interruption after sleeping user specified limit
## ThreadInterruptMonitor class
Simple implementation of [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) by starting another thread to require the interruption after sleeping user specified limit.
```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```
## Constructors
| Name | Description |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Constructs one interruption monitor. |
## Properties
| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | See [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |
## Methods
| Name | Description |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Finishes the monitor for one procedure. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |
### Remarks
One monitor instance can be used repeatedly, as long as you monitor each process in sequence. It should not be used to monitor multiple procedures concurrently in multi-threads.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThreadInterruptMonitorDemo
{
public static void ThreadInterruptMonitorExample()
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
}
}
```
### See Also
* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

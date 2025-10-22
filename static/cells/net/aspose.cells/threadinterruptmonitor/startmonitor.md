##ThreadInterruptMonitor.StartMonitor
ThreadInterruptMonitor method. Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called so the procedure which needs to be monitored should be started just after this call
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
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadInterruptMonitorMethodStartMonitorWithInt32Demo
{
public static void Run()
{
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
monitor.StartMonitor(1000);
try
{
Workbook wb = new Workbook("Large.xlsx", lopts);
monitor.FinishMonitor();
monitor.StartMonitor(1500);
wb.Save("result.xlsx");
monitor.FinishMonitor();
}
catch (Exception ex)
{
Console.WriteLine("Exception: " + ex.Message);
}
}
}
}
```
### See Also
* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

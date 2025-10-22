##SystemTimeInterruptMonitor.StartMonitor
SystemTimeInterruptMonitor method. Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called so the procedure which needs to be monitored should be started just after this call
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
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SystemTimeInterruptMonitorMethodStartMonitorWithInt32Demo
{
public static void Run()
{
SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
monitor.StartMonitor(1000); // 1 second time limit
try
{
Workbook wb = new Workbook("Large.xlsx", lopts);
monitor.StartMonitor(1500); // 1.5 second time limit
wb.Save("SystemTimeInterruptMonitorExample.xlsx");
}
catch (Exception ex)
{
Console.WriteLine("Operation interrupted: " + ex.Message);
}
}
}
}
```
### See Also
* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

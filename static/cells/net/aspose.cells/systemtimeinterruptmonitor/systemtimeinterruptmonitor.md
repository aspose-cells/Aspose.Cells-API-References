##SystemTimeInterruptMonitor.SystemTimeInterruptMonitor
SystemTimeInterruptMonitor constructor. Constructs one interruption monitor
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
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
{
public static void Run()
{
// Create an instance with terminateWithoutException set to false
SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
// Set up load options with the monitor
LoadOptions lopts = new LoadOptions();
lopts.InterruptMonitor = monitor;
// Start monitoring with 1 second time limit
monitor.StartMonitor(1000);
try
{
// Attempt to load a workbook
Workbook wb = new Workbook("sample.xlsx", lopts);
// Reset monitor for save operation with 1.5 second limit
monitor.StartMonitor(1500);
wb.Save("output.xlsx");
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

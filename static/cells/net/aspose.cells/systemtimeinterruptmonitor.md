##Class SystemTimeInterruptMonitor
Aspose.Cells.SystemTimeInterruptMonitor class. Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit
## SystemTimeInterruptMonitor class
Simple implementation of [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) by checking and comparing current system time with user specified limit.
```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```
## Constructors
| Name | Description |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Constructs one interruption monitor. |
## Properties
| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | See [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |
## Methods
| Name | Description |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |
### Remarks
This implementation is just a simple solution for simple scenarios. It needs to frequently retrieve and check the system time so itself may have a negative impact on performance to some extent.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SystemTimeInterruptMonitorDemo
{
public static void SystemTimeInterruptMonitorExample()
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
}
}
```
### See Also
* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

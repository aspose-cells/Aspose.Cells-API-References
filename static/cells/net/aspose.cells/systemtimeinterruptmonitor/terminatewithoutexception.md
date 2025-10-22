##SystemTimeInterruptMonitor.TerminateWithoutException
SystemTimeInterruptMonitor property. See TerminateWithoutException. This property is specified by user when constructing this monitor instance
## SystemTimeInterruptMonitor.TerminateWithoutException property
See [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). This property is specified by user when constructing this monitor instance.
```csharp
public override bool TerminateWithoutException { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SystemTimeInterruptMonitor with initial TerminateWithoutException value
SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
// Display the current value of the TerminateWithoutException property
Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);
// Start monitoring with a time limit of 1000ms
monitor.StartMonitor(1000);
// Demonstrate the effect of TerminateWithoutException by attempting a long operation
try
{
// Simulate a long operation that might exceed the time limit
for (int i = 0; i < 100000; i++)
{
worksheet.Cells[i, 0].Value = i;
if (monitor.IsInterruptionRequested)
{
Console.WriteLine("Operation interrupted by monitor");
break;
}
}
}
catch (Exception ex)
{
Console.WriteLine("Exception caught: " + ex.Message);
}
// Create another monitor with TerminateWithoutException set to true
SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);
// Save the workbook
workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
}
}
}
```
### See Also
* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

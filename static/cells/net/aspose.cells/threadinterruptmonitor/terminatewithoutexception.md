##ThreadInterruptMonitor.TerminateWithoutException
ThreadInterruptMonitor property. See TerminateWithoutException. This property is specified by user when constructing this monitor instance
## ThreadInterruptMonitor.TerminateWithoutException property
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
public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of ThreadInterruptMonitor with initial TerminateWithoutException value
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
// Display the current value of the property
Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);
// Start monitoring with a 5 second limit
monitor.StartMonitor(5000);
// Demonstrate processing that might be interrupted
try
{
for (int i = 0; i < 100000; i++)
{
// Simulate long processing
if (monitor.IsInterruptionRequested)
{
Console.WriteLine("Processing was interrupted");
break;
}
worksheet.Cells[i, 0].Value = "Value " + i;
}
}
catch (Exception ex)
{
Console.WriteLine("Exception occurred: " + ex.Message);
}
finally
{
monitor.FinishMonitor();
}
// Create another monitor with TerminateWithoutException set to true
ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);
// Save the result
workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

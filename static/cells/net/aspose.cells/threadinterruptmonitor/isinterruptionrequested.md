##ThreadInterruptMonitor.IsInterruptionRequested
ThreadInterruptMonitor property. This implementation just checks whether the time costfrom the time when starting this monitor to now is greater than user specified limit
## ThreadInterruptMonitor.IsInterruptionRequested property
This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.
```csharp
public override bool IsInterruptionRequested { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Threading;
public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of ThreadInterruptMonitor
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);
// Start monitoring with a 2-second limit
monitor.StartMonitor(2000);
// Simulate a long-running operation
Console.WriteLine("Starting long operation...");
for (int i = 0; i < 100; i++)
{
// Check if interruption was requested
if (monitor.IsInterruptionRequested)
{
Console.WriteLine("Operation was interrupted!");
break;
}
// Simulate work
Thread.Sleep(100);
worksheet.Cells[i, 0].Value = $"Processed row {i}";
Console.WriteLine($"Processed row {i}");
}
// Finish monitoring
monitor.FinishMonitor();
// Save the result
workbook.Save("ThreadInterruptionDemo.xlsx");
}
}
}
```
### See Also
* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

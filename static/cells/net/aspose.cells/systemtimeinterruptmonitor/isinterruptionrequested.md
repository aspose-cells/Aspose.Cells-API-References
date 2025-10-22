##SystemTimeInterruptMonitor.IsInterruptionRequested
SystemTimeInterruptMonitor property. This implementation just checks whether the time costfrom the time when starting this monitor to now is greater than user specified limit
## SystemTimeInterruptMonitor.IsInterruptionRequested property
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
public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SystemTimeInterruptMonitor
SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
// Start monitoring with a 5-second time limit
monitor.StartMonitor(5000);
// Display initial IsInterruptionRequested value
Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);
// Simulate long-running operation
Console.WriteLine("Starting long operation...");
for (int i = 0; i < 100000; i++)
{
worksheet.Cells[i, 0].Value = i;
// Check if interruption was requested
if (monitor.IsInterruptionRequested)
{
Console.WriteLine("Operation interrupted after time limit!");
break;
}
}
// Display final IsInterruptionRequested value
Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);
// Save the result
workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
}
}
}
```
### See Also
* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

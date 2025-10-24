##AbstractInterruptMonitor.TerminateWithoutException
AbstractInterruptMonitor property. When procedure is interrupted whether terminate the procedure quietly or throw an Exception. Default is false that is when IsInterruptionRequested is true a CellsException with code Interrupted will be thrown
## AbstractInterruptMonitor.TerminateWithoutException property
When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [`IsInterruptionRequested`](../isinterruptionrequested/) is true, a [`CellsException`](../../cellsexception/) with code Interrupted will be thrown.
```csharp
public virtual bool TerminateWithoutException { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AbstractInterruptMonitorPropertyTerminateWithoutExceptionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet to create processing workload
for (int row = 0; row < 5000; row++)
{
for (int col = 0; col < 50; col++)
{
worksheet.Cells[row, col].Value = "SampleData";
}
}
// Demonstrate SystemTimeInterruptMonitor with exception termination
var interruptMonitor1 = new SystemTimeInterruptMonitor(terminateWithoutException: false);
Console.WriteLine($"Initial TerminateWithoutException: {interruptMonitor1.TerminateWithoutException}");
workbook.InterruptMonitor = interruptMonitor1;
interruptMonitor1.StartMonitor(1); // Set 1ms timeout
try
{
workbook.Save("TerminateWithException.xlsx");
Console.WriteLine("Saved successfully (unexpected with false setting)");
}
catch (CellsException ex)
{
Console.WriteLine($"Operation terminated with exception: {ex.Message}");
}
// Demonstrate SystemTimeInterruptMonitor with silent termination
var interruptMonitor2 = new SystemTimeInterruptMonitor(terminateWithoutException: true);
Console.WriteLine($"\nNew TerminateWithoutException: {interruptMonitor2.TerminateWithoutException}");
workbook.InterruptMonitor = interruptMonitor2;
interruptMonitor2.StartMonitor(1);
try
{
workbook.Save("TerminateSilently.xlsx");
Console.WriteLine("Saved without exception (expected with true setting)");
}
catch (CellsException)
{
Console.WriteLine("Exception caught (unexpected with true setting)");
}
}
}
}
```
### See Also
* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

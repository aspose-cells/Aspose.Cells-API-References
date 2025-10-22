##InterruptMonitor.IsInterruptionRequested
InterruptMonitor property. Mark the monitor as requesting interruption
## InterruptMonitor.IsInterruptionRequested property
Mark the monitor as requesting interruption
```csharp
public override bool IsInterruptionRequested { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class InterruptMonitorPropertyIsInterruptionRequestedDemo
{
public static void Run()
{
// Create a new workbook and access its first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an interrupt monitor and assign it to workbook
InterruptMonitor monitor = new InterruptMonitor();
workbook.InterruptMonitor = monitor;
// Display initial state of IsInterruptionRequested
Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);
// Simulate a long-running data processing operation
Console.WriteLine("Starting data processing...");
for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
{
// Request interruption after processing 500 rows
if (rowIdx == 500)
{
monitor.Interrupt();
Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
}
// Check for interruption request
if (monitor.IsInterruptionRequested)
{
Console.WriteLine($"Processing interrupted at row {rowIdx}");
break;
}
// Simulate data processing
worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
}
// Save the modified workbook
workbook.Save("InterruptionDemoOutput.xlsx");
Console.WriteLine("File saved with partial data due to interruption.");
}
}
}
```
### See Also
* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

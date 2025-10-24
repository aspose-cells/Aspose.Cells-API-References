##Workbook.InterruptMonitor
Workbook property. Gets and sets the interrupt monitor
## Workbook.InterruptMonitor property
Gets and sets the interrupt monitor.
```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyInterruptMonitorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some data to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Create and assign interrupt monitor
InterruptMonitor monitor = new InterruptMonitor();
workbook.InterruptMonitor = monitor;
try
{
Console.WriteLine("Starting save operation...");
// Simulate a long-running operation by interrupting immediately
monitor.Interrupt();
// Attempt to save - should be interrupted
workbook.Save("output.pdf", SaveFormat.Pdf);
Console.WriteLine("Save completed successfully.");
}
catch (CellsException e)
{
if (e.Code == ExceptionType.Interrupted)
{
Console.WriteLine("Operation was successfully interrupted.");
}
else
{
Console.WriteLine($"Error occurred: {e.Message}");
}
}
}
}
}
```
### See Also
* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

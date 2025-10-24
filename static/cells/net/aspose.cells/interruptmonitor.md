##Class InterruptMonitor
Aspose.Cells.InterruptMonitor class. Represents all operator about the interrupt
## InterruptMonitor class
Represents all operator about the interrupt.
```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```
## Constructors
| Name | Description |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Mark the monitor as requesting interruption |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) is true, a [`CellsException`](../cellsexception/) with code Interrupted will be thrown.(Inherited from [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |
## Methods
| Name | Description |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Interrupt the current operator. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassInterruptMonitorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Create and assign interrupt monitor
InterruptMonitor monitor = new InterruptMonitor();
workbook.InterruptMonitor = monitor;
try
{
Console.WriteLine("Starting save operation...");
// Simulate interrupting the operation
monitor.Interrupt();
// Attempt to save (should be interrupted)
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
Console.WriteLine("Error occurred: " + e.Message);
}
}
}
}
}
```
### See Also
* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

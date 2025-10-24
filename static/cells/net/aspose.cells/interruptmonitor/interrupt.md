##InterruptMonitor.Interrupt
InterruptMonitor method. Interrupt the current operator
## InterruptMonitor.Interrupt method
Interrupt the current operator.
```csharp
public void Interrupt()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class InterruptMonitorMethodInterruptDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some data to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 10000; i++)
{
worksheet.Cells[i, 0].Value = "Data " + i;
}
// Create and set interrupt monitor
InterruptMonitor monitor = new InterruptMonitor();
workbook.InterruptMonitor = monitor;
try
{
Console.WriteLine("Starting long operation...");
// Simulate a long operation in another thread
System.Threading.ThreadPool.QueueUserWorkItem(_ =>
{
System.Threading.Thread.Sleep(1000); // Wait 1 second
Console.WriteLine("Interrupting operation...");
monitor.Interrupt(); // Call interrupt
});
// Perform a long operation (save)
workbook.Save("output.pdf", SaveFormat.Pdf);
Console.WriteLine("Operation completed successfully.");
}
catch (CellsException e)
{
if (e.Code == ExceptionType.Interrupted)
{
Console.WriteLine("Operation was interrupted successfully.");
}
else
{
Console.WriteLine("Error: " + e.Message);
}
}
}
}
}
```
### See Also
* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

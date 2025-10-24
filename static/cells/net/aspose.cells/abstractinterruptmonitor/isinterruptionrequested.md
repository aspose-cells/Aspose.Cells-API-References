##AbstractInterruptMonitor.IsInterruptionRequested
AbstractInterruptMonitor property. Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here otherwise it may become another bottleneck for the procedure
## AbstractInterruptMonitor.IsInterruptionRequested property
Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure.
```csharp
public abstract bool IsInterruptionRequested { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Threading;
using System.Threading.Tasks;
public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create interrupt monitor and assign to workbook
InterruptMonitor monitor = new InterruptMonitor();
workbook.InterruptMonitor = monitor;
// Display initial value
Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);
// Start interruption task
Task.Run(() =>
{
Thread.Sleep(1000); // Wait 1 seconds
Console.WriteLine("\nTriggering interruption...");
monitor.Interrupt();
});
// Long-running operation simulation
Console.WriteLine("Starting data generation...");
try
{
for (int i = 0; i < 500000000; i++)
{
if (monitor.IsInterruptionRequested)
{
Console.WriteLine($"\nInterrupted at row {i}");
break;
}
worksheet.Cells[i, 0].Value = $"Data {i}";
// Simulate processing time
if (i % 1000 == 0)
Console.Write(".");
}
}
catch (Exception ex)
{
Console.WriteLine("\nError: " + ex.Message);
}
// Save result
workbook.Save("InterruptionDemoOutput.xlsx");
Console.WriteLine("\nWorkbook saved with partial data.");
}
}
}
```
### See Also
* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

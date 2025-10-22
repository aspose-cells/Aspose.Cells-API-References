##ThreadInterruptMonitor.ThreadInterruptMonitor
ThreadInterruptMonitor constructor. Constructs one interruption monitor
## ThreadInterruptMonitor constructor
Constructs one interruption monitor.
```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```
| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a ThreadInterruptMonitor with throwOnInterrupted set to false
ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
workbook.InterruptMonitor = monitor;
// Set a short time limit (100ms) for demonstration
int timeLimit = 100;
monitor.StartMonitor(timeLimit);
try
{
// Perform a long operation (will be interrupted)
for (int i = 0; i < 100000; i++)
{
workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
}
Console.WriteLine("Operation completed without interruption");
}
catch (CellsException e)
{
if (e.Code == ExceptionType.Interrupted)
{
Console.WriteLine("Operation was successfully interrupted");
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
* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

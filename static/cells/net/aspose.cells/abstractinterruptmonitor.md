##Class AbstractInterruptMonitor
Aspose.Cells.AbstractInterruptMonitor class. Monitor for interruption requests in all timeconsuming operations
## AbstractInterruptMonitor class
Monitor for interruption requests in all time-consuming operations.
```csharp
public abstract class AbstractInterruptMonitor
```
## Properties
| Name | Description |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [`IsInterruptionRequested`](./isinterruptionrequested/) is true, a [`CellsException`](../cellsexception/) with code Interrupted will be thrown. |
### Examples
```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;
namespace AsposeCellsExamples
{
// Custom implementation of AbstractInterruptMonitor
public class CustomInterruptMonitor : AbstractInterruptMonitor
{
//the result file is correct
public override bool IsInterruptionRequested
{
get
{
Console.WriteLine("Get the return value of whether to interrupt the program===");
// Logic to determine if interruption is requested
return false; // Change this based on your logic
}
}
public override bool TerminateWithoutException
{
get => false; // Change this based on your logic
}
//// the result file crashes
//public override bool IsInterruptionRequested
//{
//    get
//    {
//        Console.WriteLine("Get the return value of whether to interrupt the program===");
//        // Logic to determine if interruption is requested
//        //return false; // Change this based on your logic
//        return true;
//    }
//}
//public override bool TerminateWithoutException
//{
//    get => true; // Change this based on your logic
//}
}
public class InterruptMonitorDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(20);
sheet.Cells["A3"].Formula = "=A1+A2";
// Create an instance of CustomInterruptMonitor
CustomInterruptMonitor monitor = new CustomInterruptMonitor();
// Set load options with the custom interrupt monitor
LoadOptions loadOptions = new LoadOptions
{
InterruptMonitor = monitor
};
// Load the workbook with the specified options
workbook = new Workbook("Sample.xlsx", loadOptions);
// Perform calculations
workbook.CalculateFormula();
// Save the workbook
workbook.Save("InterruptMonitorDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

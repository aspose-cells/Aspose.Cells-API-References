##IWarningCallback.Warning
IWarningCallback method. Our callback only needs to implement the Warning method
## IWarningCallback.Warning method
Our callback only needs to implement the "Warning" method.
```csharp
public void Warning(WarningInfo warningInfo)
```
| Parameter | Type | Description |
| --- | --- | --- |
| warningInfo | WarningInfo | warning info |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IWarningCallbackMethodWarningWithWarningInfoDemo : IWarningCallback
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var demo = new IWarningCallbackMethodWarningWithWarningInfoDemo();
workbook.Settings.WarningCallback = demo;
try
{
Console.WriteLine("Warning callback is set up. Any warnings during operations will be displayed.");
// Demonstrate effect by saving with a potential warning scenario
worksheet.Cells["A1"].Formula = "=1/0"; // This may trigger a warning
workbook.Save("WarningDemoOutput.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
public void Warning(WarningInfo warningInfo)
{
Console.WriteLine($"Warning Type: {warningInfo.Type}");
Console.WriteLine($"Description: {warningInfo.Description}");
Console.WriteLine($"Corrected Object: {warningInfo.CorrectedObject ?? "null"}");
}
}
}
```
### See Also
* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

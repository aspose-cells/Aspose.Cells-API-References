##Name.IsReferred
Name property. Indicates whether this name is referred by other formulas
## Name.IsReferred property
Indicates whether this name is referred by other formulas.
```csharp
public bool IsReferred { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NamePropertyIsReferredDemo
{
public static void Run()
{
Workbook wb = new Workbook();
NameCollection nc = wb.Worksheets.Names;
// Add names
Name n1 = nc[nc.Add("TestName1")];
n1.RefersTo = "=Sheet1!F10:G15";
Name n2 = nc[nc.Add("TestName2")];
n2.RefersTo = "=Sheet1!H10:I15";
// Add worksheet-scoped names
Name n3 = nc[nc.Add("Sheet1!TestName1")];
n3.RefersTo = "=Sheet1!F20:G25";
Name n4 = nc[nc.Add("Sheet1!TestName2")];
n4.RefersTo = "=Sheet1!H20:I25";
// Create formulas that reference the names
wb.Worksheets.Add();
wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";
// Demonstrate IsReferred property
Console.WriteLine($"TestName1.IsReferred: {n1.IsReferred}"); // False
Console.WriteLine($"Sheet1!TestName1.IsReferred: {n3.IsReferred}"); // False
Console.WriteLine($"TestName2.IsReferred: {n2.IsReferred}"); // True
Console.WriteLine($"Sheet1!TestName2.IsReferred: {n4.IsReferred}"); // True
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

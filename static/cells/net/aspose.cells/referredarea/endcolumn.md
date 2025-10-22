##ReferredArea.EndColumn
ReferredArea property. The end column of the area
## ReferredArea.EndColumn property
The end column of the area.
```csharp
public int EndColumn { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyEndColumnDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["B2"];
cell.Formula = "=SUM(A1:C3)";
ReferredAreaCollection referredAreas = cell.GetPrecedents();
foreach (ReferredArea area in referredAreas)
{
Console.WriteLine($"StartColumn: {area.StartColumn}");
Console.WriteLine($"EndColumn: {area.EndColumn}");
Console.WriteLine($"Columns spanned: {area.EndColumn - area.StartColumn + 1}");
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

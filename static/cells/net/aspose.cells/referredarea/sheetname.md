##ReferredArea.SheetName
ReferredArea property. Indicates which sheet this reference is in
## ReferredArea.SheetName property
Indicates which sheet this reference is in.
```csharp
public string SheetName { get; }
```
### Remarks
If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertySheetNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
Worksheet worksheet1 = workbook.Worksheets["Sheet1"];
workbook.Worksheets["Sheet2"].Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
ReferredArea ra = worksheet1.Cells["A1"].GetPrecedents()[0];
Console.WriteLine("Precedent's referred sheet: " + ra.SheetName);
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

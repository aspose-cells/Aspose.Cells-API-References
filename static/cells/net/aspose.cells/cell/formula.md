##Cell.Formula
Cell property. Gets or sets a formula of the Cell
## Cell.Formula property
Gets or sets a formula of the [`Cell`](../).
```csharp
public string Formula { get; set; }
```
### Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyFormulaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values in cells that will be used in the formula
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
worksheet.Cells["E1"].PutValue(5);
worksheet.Cells["A1"].PutValue(100);
// Set formula in cell B6
worksheet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + A1";
// Calculate the formula
workbook.CalculateFormula();
// Display the result
Console.WriteLine("Formula result in B6: " + worksheet.Cells["B6"].Value);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

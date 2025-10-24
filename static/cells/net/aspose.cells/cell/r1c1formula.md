##Cell.R1C1Formula
Cell property. Gets or sets a R1C1 formula of the Cell
## Cell.R1C1Formula property
Gets or sets a R1C1 formula of the [`Cell`](../).
```csharp
public string R1C1Formula { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyR1C1FormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set A1 value
worksheet.Cells["A1"].PutValue(10);
// Set B1 value
worksheet.Cells["B1"].PutValue(20);
// Set C1 formula in A1 notation
worksheet.Cells["C1"].Formula = "=A1+B1";
// Get and display R1C1 formula
string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
Console.WriteLine("R1C1 Formula: " + r1c1Formula);
// Set D1 formula in R1C1 notation
worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
// Get and display A1 formula
string a1Formula = worksheet.Cells["D1"].Formula;
Console.WriteLine("A1 Formula: " + a1Formula);
// Save the workbook
workbook.Save("R1C1FormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

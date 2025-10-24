##Range.Transpose
Range method. Transpose rotate data from rows to columns or vice versa
## Range.Transpose method
Transpose (rotate) data from rows to columns or vice versa.
```csharp
public void Transpose()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodTransposeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Fill sample data in a 3x3 range (A1:C3)
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["B1"].PutValue(2);
worksheet.Cells["C1"].PutValue(3);
worksheet.Cells["A2"].PutValue(4);
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["C2"].PutValue(6);
worksheet.Cells["A3"].PutValue(7);
worksheet.Cells["B3"].PutValue(8);
worksheet.Cells["C3"].PutValue(9);
// Create a range (A1:C3)
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
// Transpose the range
range.Transpose();
// Save the workbook
workbook.Save("TransposedOutput.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

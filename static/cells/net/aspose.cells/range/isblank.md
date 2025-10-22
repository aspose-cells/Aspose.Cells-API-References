##Range.IsBlank
Range method. Indicates whether the range contains values
## Range.IsBlank method
Indicates whether the range contains values.
```csharp
public bool IsBlank()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodIsBlankDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a range and check if it's blank (should be true)
Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());
// Put a value in one cell and check again (should be false)
cells["B2"].PutValue("Test");
Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

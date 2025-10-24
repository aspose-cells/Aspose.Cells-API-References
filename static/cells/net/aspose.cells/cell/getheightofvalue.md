##Cell.GetHeightOfValue
Cell method. Gets the height of the value in unit of pixels
## Cell.GetHeightOfValue method
Gets the height of the value in unit of pixels.
```csharp
public int GetHeightOfValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetHeightOfValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set value and measure height
worksheet.Cells["A1"].PutValue("Sample Text");
double height = worksheet.Cells["A1"].GetHeightOfValue();
Console.WriteLine("Height of value in A1: " + height);
// Adjust row height and measure again
worksheet.Cells.Rows[0].Height = 30;
height = worksheet.Cells["A1"].GetHeightOfValue();
Console.WriteLine("Height after row adjustment: " + height);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

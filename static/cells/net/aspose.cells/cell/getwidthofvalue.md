##Cell.GetWidthOfValue
Cell method. Gets the width of the value in unit of pixels
## Cell.GetWidthOfValue method
Gets the width of the value in unit of pixels.
```csharp
public int GetWidthOfValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetWidthOfValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("CellsJava40307");
int width = cell.GetWidthOfValue();
Console.WriteLine("Width of the cell value: " + width);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

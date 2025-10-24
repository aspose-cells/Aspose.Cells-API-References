##Cells.ConvertStringToNumericValue
Cells method. Converts all string data in the worksheet to numeric value if possible
## Cells.ConvertStringToNumericValue method
Converts all string data in the worksheet to numeric value if possible.
```csharp
public void ConvertStringToNumericValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodConvertStringToNumericValueDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Cells cells = wb.Worksheets[0].Cells;
// Put string values that can be converted to numeric values
cells[0, 0].PutValue("1.23");
cells[0, 1].PutValue("1.24");
cells[0, 2].PutValue("1.23");
cells[0, 3].PutValue("6/20/2021");
cells[0, 4].PutValue("def"); // This will remain as string
cells[0, 5].PutValue("6/20/2021");
// Convert string values to numeric where possible
cells.ConvertStringToNumericValue();
// Display the converted values
Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

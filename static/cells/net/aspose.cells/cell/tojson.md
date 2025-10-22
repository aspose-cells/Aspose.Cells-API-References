##Cell.ToJson
Cell method. Convert Cell to JSON struct data
## Cell.ToJson method
Convert [`Cell`](../) to JSON struct data.
```csharp
public string ToJson()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodToJsonDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set sample data and styles
cells["A1"].PutValue(100);
cells["B6"].Formula = "=A1";
// Get cell and convert to JSON
Cell cell = cells["B6"];
string json = cell.ToJson();
// Output the JSON
Console.WriteLine("Cell JSON:");
Console.WriteLine(json);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

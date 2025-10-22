##FindOptions.GetRange
FindOptions method. Gets and sets the searched range
## FindOptions.GetRange method
Gets and sets the searched range.
```csharp
public CellArea GetRange()
```
### Return Value
Returns the searched range.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FindOptionsMethodGetRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Cherry");
worksheet.Cells["B1"].PutValue("Orange");
worksheet.Cells["B2"].PutValue("Grape");
worksheet.Cells["B3"].PutValue("Lemon");
// Create FindOptions instance
FindOptions findOptions = new FindOptions();
findOptions.LookInType = LookInType.Values;
findOptions.LookAtType = LookAtType.Contains;
// Set the search range to A1:B3
CellArea searchArea = new CellArea();
searchArea.StartRow = 0;
searchArea.StartColumn = 0;
searchArea.EndRow = 2;
searchArea.EndColumn = 1;
findOptions.SetRange(searchArea);
try
{
// Get the range that was set
CellArea resultRange = findOptions.GetRange();
// Display the range information
Console.WriteLine($"Search range: StartRow={resultRange.StartRow}, StartColumn={resultRange.StartColumn}, " +
$"EndRow={resultRange.EndRow}, EndColumn={resultRange.EndColumn}");
// Perform a find operation to demonstrate the range is being used
Cell foundCell = worksheet.Cells.Find("an", null, findOptions);
if (foundCell != null)
{
Console.WriteLine($"Found value '{foundCell.StringValue}' at {foundCell.Name}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRange method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

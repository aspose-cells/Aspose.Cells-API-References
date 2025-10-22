##FindOptions.ValueTypeSensitive
FindOptions property. Indicates whether searched cell value type should be same with the searched key
## FindOptions.ValueTypeSensitive property
Indicates whether searched cell value type should be same with the searched key.
```csharp
public bool ValueTypeSensitive { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyValueTypeSensitiveDemo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add different value types to cells
worksheet.Cells["A1"].PutValue("100"); // Stored as string
worksheet.Cells["A2"].PutValue(100);   // Stored as number
worksheet.Cells["A3"].PutValue("100.0"); // Stored as string
worksheet.Cells["A4"].PutValue(100.0);   // Stored as number
// Create find options with ValueTypeSensitive = true
FindOptions options = new FindOptions();
options.ValueTypeSensitive = true;
options.LookAtType = LookAtType.EntireContent;
// Search for number 100 (won't find string "100")
Cell foundCell = worksheet.Cells.Find(100, null, options);
Console.WriteLine("Found cell with number 100: " + (foundCell != null ? foundCell.Name : "Not found"));
// Search for string "100" (won't find number 100)
foundCell = worksheet.Cells.Find("100", null, options);
Console.WriteLine("Found cell with string \"100\": " + (foundCell != null ? foundCell.Name : "Not found"));
// Change to ValueTypeSensitive = false
options.ValueTypeSensitive = false;
// Now both searches will find any cell with "100" or 100
foundCell = worksheet.Cells.Find(100, null, options);
Console.WriteLine("Found any 100 (type insensitive): " + (foundCell != null ? foundCell.Name : "Not found"));
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

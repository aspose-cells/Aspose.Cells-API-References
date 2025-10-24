##FindOptions.ConvertNumericData
FindOptions property. Gets or sets a value that indicates whether converting the searched string value to numeric data
## FindOptions.ConvertNumericData property
Gets or sets a value that indicates whether converting the searched string value to numeric data.
```csharp
public bool ConvertNumericData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyConvertNumericDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data including numeric values as strings
worksheet.Cells["A1"].PutValue("123");
worksheet.Cells["A2"].PutValue("456");
worksheet.Cells["A3"].PutValue("01/28/2010");
// Create find options and set ConvertNumericData to true
FindOptions options = new FindOptions();
options.ConvertNumericData = true;
// Find the date value (stored as string but converted to numeric during search)
Cell foundCell = worksheet.Cells.Find("01/28/2010", null, options);
// Output the result
if (foundCell != null)
{
Console.WriteLine("Found value at: " + foundCell.Name);
Console.WriteLine("Cell value: " + foundCell.StringValue);
}
else
{
Console.WriteLine("Value not found");
}
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

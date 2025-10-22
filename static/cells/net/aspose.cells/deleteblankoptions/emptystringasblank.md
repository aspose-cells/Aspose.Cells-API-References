##DeleteBlankOptions.EmptyStringAsBlank
DeleteBlankOptions property. Whether one cell will be taken as blank when its value is empty string. Default value is true
## DeleteBlankOptions.EmptyStringAsBlank property
Whether one cell will be taken as blank when its value is empty string. Default value is true.
```csharp
public bool EmptyStringAsBlank { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet with data including empty strings
worksheet.Cells["A1"].PutValue("Data");
worksheet.Cells["A2"].PutValue("");
worksheet.Cells["A3"].PutValue("More Data");
worksheet.Cells["A4"].PutValue("");
worksheet.Cells["A5"].PutValue("Even More Data");
// Configure DeleteBlankOptions with EmptyStringAsBlank set to true
DeleteBlankOptions options = new DeleteBlankOptions
{
EmptyStringAsBlank = true
};
// Delete rows containing empty strings (treated as blanks)
worksheet.Cells.DeleteBlankRows(options);
// Save the result
workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
}
}
}
```
### See Also
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

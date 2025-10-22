##Worksheet.UniqueId
Worksheet property. Gets and sets the unique id it is same as 15DB5C3CA5A148AF8F253D86AC232D4F
## Worksheet.UniqueId property
Gets and sets the unique id, it is same as {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.
```csharp
public string UniqueId { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyUniqueIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Generate a unique ID for the worksheet
string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
// Set the UniqueId property of the first worksheet
workbook.Worksheets[0].UniqueId = uniqueId;
// Save the workbook
string outputPath = "SheetUniqueIdDemo.xlsx";
workbook.Save(outputPath);
// Reload the workbook to verify the UniqueId persists
Workbook loadedWorkbook = new Workbook(outputPath);
// Output the UniqueId to demonstrate functionality
Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

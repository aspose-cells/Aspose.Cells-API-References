##ListObject.AlternativeDescription
ListObject property. Gets and sets the alternative description
## ListObject.AlternativeDescription property
Gets and sets the alternative description.
```csharp
public string AlternativeDescription { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyAlternativeDescriptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = worksheet.ListObjects[index];
// Set alternative text and description
listObject.AlternativeText = "Test";
listObject.AlternativeDescription = "aSXADCS";
// Save the workbook
workbook.Save("output.xlsx");
// Reload and verify the properties
Workbook loadedWorkbook = new Workbook("output.xlsx");
ListObject loadedListObject = loadedWorkbook.Worksheets[0].ListObjects[0];
Console.WriteLine("AlternativeText: " + loadedListObject.AlternativeText);
Console.WriteLine("AlternativeDescription: " + loadedListObject.AlternativeDescription);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

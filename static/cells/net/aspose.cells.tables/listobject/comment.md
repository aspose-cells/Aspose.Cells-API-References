##ListObject.Comment
ListObject property. Gets and sets the comment of the table
## ListObject.Comment property
Gets and sets the comment of the table.
```csharp
public string Comment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyCommentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for the list object
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(100);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
ListObject listObj = worksheet.ListObjects[index];
// Set and demonstrate the Comment property
listObj.Comment = "This is a sample comment for the list object";
Console.WriteLine("List Object Comment: " + listObj.Comment);
// Resize the list object to include more data
listObj.Resize(0, 0, 2, 1, true);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue(200);
// Save the workbook
workbook.Save("ListObjectCommentDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

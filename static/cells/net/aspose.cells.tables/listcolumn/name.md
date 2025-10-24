##ListColumn.Name
ListColumn property. Gets and sets the name of the column
## ListColumn.Name property
Gets and sets the name of the column.
```csharp
public string Name { get; set; }
```
### Remarks
If sets the name of the column, the according cell' value will be changed too.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["C1"].PutValue("Value");
// Create a table/list object
int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];
// Access and modify the Name property of the first list column
listObject.ListColumns[0].Name = "NewID";
// Verify the name was set
Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
// Save the workbook
workbook.Save("ListColumnPropertyNameDemo.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

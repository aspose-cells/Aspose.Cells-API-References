##ListObject.StartRow
ListObject property. Gets the start row of the range
## ListObject.StartRow property
Gets the start row of the range.
```csharp
public int StartRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyStartRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data starting from row 2
worksheet.Cells["A2"].PutValue("ID");
worksheet.Cells["B2"].PutValue("Name");
worksheet.Cells["A3"].PutValue(1);
worksheet.Cells["B3"].PutValue("John");
worksheet.Cells["A4"].PutValue(2);
worksheet.Cells["B4"].PutValue("Mary");
// Create a list object starting from row 2
int listObjectIndex = worksheet.ListObjects.Add(1, 0, 3, 1, true);
ListObject listObject = worksheet.ListObjects[listObjectIndex];
// Display the StartRow property
Console.WriteLine("ListObject StartRow: " + listObject.StartRow);
// To "modify" the start row, we need to recreate the ListObject
worksheet.ListObjects.RemoveAt(listObjectIndex);
listObjectIndex = worksheet.ListObjects.Add(2, 0, 3, 1, true);
listObject = worksheet.ListObjects[listObjectIndex];
Console.WriteLine("Modified ListObject StartRow: " + listObject.StartRow);
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

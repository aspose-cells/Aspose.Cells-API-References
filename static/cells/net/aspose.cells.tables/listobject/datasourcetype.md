##ListObject.DataSourceType
ListObject property. Gets the data source type of the table
## ListObject.DataSourceType property
Gets the data source type of the table.
```csharp
public TableDataSourceType DataSourceType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyDataSourceTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["B3"].PutValue("Bob");
// Create list object and get it from the collection
int listObjectIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = worksheet.ListObjects[listObjectIndex];
listObject.DisplayName = "EmployeeTable";
// Get and display DataSourceType
TableDataSourceType dataSourceType = listObject.DataSourceType;
Console.WriteLine("ListObject DataSourceType: " + dataSourceType);
workbook.Save("ListObjectDataSourceTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TableDataSourceType](../../tabledatasourcetype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

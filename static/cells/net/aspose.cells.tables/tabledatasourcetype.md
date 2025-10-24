##Enum TableDataSourceType
Aspose.Cells.Tables.TableDataSourceType enum. Represents the tables data source type
## TableDataSourceType enumeration
Represents the table's data source type.
```csharp
public enum TableDataSourceType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Worksheet | `0` | Excel Worksheet Table |
| SharePoint | `1` | Read-write SharePoint linked List |
| XML | `2` | XML mapper Table |
| QueryTable | `3` | Query Table |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableDataSourceTypeDemo
{
public static void TableDataSourceTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("ID");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["B2"].PutValue("Alice");
worksheet.Cells["B3"].PutValue("Bob");
worksheet.Cells["B4"].PutValue("Charlie");
// Add a ListObject (table) to the worksheet
int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
ListObject listObject = worksheet.ListObjects[listObjectIndex];
// Set the display name of the table
listObject.DisplayName = "SampleTable";
// Set the data source type of the table
TableDataSourceType dataSourceType = listObject.DataSourceType;
// Output the data source type
Console.WriteLine("Data Source Type: " + dataSourceType);
// Save the workbook
workbook.Save("TableDataSourceTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)

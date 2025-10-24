##ListObject.TableStyleType
ListObject property. Gets and the builtin table style
## ListObject.TableStyleType property
Gets and the built-in table style.
```csharp
public TableStyleType TableStyleType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyTableStyleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
}
}
// Get the list objects collection
ListObjectCollection tables = worksheet.ListObjects;
// Add a table
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
// Set the table style
table.TableStyleType = TableStyleType.TableStyleDark2;
// Save the workbook
workbook.Save("TableStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

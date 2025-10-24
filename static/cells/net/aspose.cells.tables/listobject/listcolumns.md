##ListObject.ListColumns
ListObject property. Gets ListColumns of the ListObject
## ListObject.ListColumns property
Gets ListColumns of the ListObject.
```csharp
public ListColumnCollection ListColumns { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyListColumnsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
}
}
// Create a list object
ListObjectCollection listObjects = worksheet.ListObjects;
int index = listObjects.Add(0, 0, 9, 4, true);
ListObject listObject = listObjects[index];
// Enable totals and set calculation for the 5th column
listObject.ShowTotals = true;
listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
// Apply table style
listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;
// Save the workbook
workbook.Save("ListColumnsDemo_out.xlsx");
}
}
}
```
### See Also
* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

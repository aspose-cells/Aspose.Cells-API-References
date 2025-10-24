##ListObject.ConvertToRange
ListObject method. Convert the table to range
## ConvertToRange() {#converttorange}
Convert the table to range.
```csharp
public void ConvertToRange()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodConvertToRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("ID");
sheet.Cells["B1"].PutValue("Name");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["B2"].PutValue("John");
sheet.Cells["A3"].PutValue(2);
sheet.Cells["B3"].PutValue("Mary");
// Create a list object
int index = sheet.ListObjects.Add("A1", "B3", true);
ListObject listObject = sheet.ListObjects[index];
Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
// Convert list object to range
listObject.ConvertToRange();
Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
// Save the workbook
workbook.Save("ListObjectConversion.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## ConvertToRange(TableToRangeOptions) {#converttorange_1}
Convert the table to range.
```csharp
public void ConvertToRange(TableToRangeOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | TableToRangeOptions | the options when converting table to range. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodConvertToRangeWithTableToRangeOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
for (int i = 0; i < 5; i++)
{
worksheet.Cells[0, i].PutValue($"Column {i + 1}");
for (int row = 1; row < 5; row++)
{
worksheet.Cells[row, i].PutValue(row * (i + 1));
}
}
// Create table
int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowTotals = true;
table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
// Convert table to range with options
TableToRangeOptions options = new TableToRangeOptions();
options.LastRow = 4;
table.ConvertToRange(options);
workbook.Save("TableToRangeWithOptions.xlsx");
}
}
}
```
### See Also
* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

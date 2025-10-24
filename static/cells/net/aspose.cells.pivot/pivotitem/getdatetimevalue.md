##PivotItem.GetDateTimeValue
PivotItem method. Gets the date time value of the pivot item If the value is null it will return DateTime.MinValue
## PivotItem.GetDateTimeValue method
Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue
```csharp
public DateTime GetDateTimeValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemMethodGetDateTimeValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with a date value
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
worksheet.Cells["A3"].PutValue(DateTime.Now);
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
foreach (PivotItem pivotItem in pivotItems)
{
Console.WriteLine("Pivot Item Name: " + pivotItem.Name);
DateTime dateTimeValue = pivotItem.GetDateTimeValue();
Console.WriteLine("DateTime Value: " + dateTimeValue);
}
workbook.Save("PivotItemGetDateTimeValueDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

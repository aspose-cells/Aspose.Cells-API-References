##PivotDateTimeRangeGroupSettings.End
PivotDateTimeRangeGroupSettings property. Gets the end date time of the group
## PivotDateTimeRangeGroupSettings.End property
Gets the end date time of the group.
```csharp
public DateTime End { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotDateTimeRangeGroupSettingsPropertyEndDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Date");
Style style = workbook.CreateStyle();
style.Number = 14;
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A2"].SetStyle(style);
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A3"].SetStyle(style);
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["A4"].SetStyle(style);
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField dateField = pivotTable.RowFields[0];
DateTime endDate = new DateTime(2023, 12, 31);
dateField.GroupBy(new DateTime(2023, 1, 1), endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);
PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
Console.WriteLine("End Date: " + groupSettings.End);
workbook.Save("PivotDateTimeRangeGroupSettingsEndDemo.xlsx");
}
}
}
```
### See Also
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

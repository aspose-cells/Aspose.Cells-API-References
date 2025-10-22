##PivotShowValuesSetting.BaseItemPositionType
PivotShowValuesSetting property. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for readif you need to set PivotItemPosition.Custom please set PivotField.BaseItemIndex attribute
## PivotShowValuesSetting.BaseItemPositionType property
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.
```csharp
public PivotItemPositionType BaseItemPositionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotShowValuesSettingPropertyBaseItemPositionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].Value = "Product";
worksheet.Cells[0, 1].Value = "Sales";
worksheet.Cells[1, 0].Value = "A";
worksheet.Cells[1, 1].Value = 100;
worksheet.Cells[2, 0].Value = "B";
worksheet.Cells[2, 1].Value = 150;
worksheet.Cells[3, 0].Value = "C";
worksheet.Cells[3, 1].Value = 200;
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField dataField = pivotTable.DataFields[0];
PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;
showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
showValuesSetting.BaseFieldIndex = 0;
showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
showValuesSetting.BaseItemIndex = 1;
pivotTable.RefreshData();
pivotTable.CalculateData();
workbook.Save("PivotShowValuesSettingExample.xlsx");
}
}
}
```
### See Also
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

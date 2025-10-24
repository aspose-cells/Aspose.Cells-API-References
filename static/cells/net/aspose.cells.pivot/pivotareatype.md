##Enum PivotAreaType
Aspose.Cells.Pivot.PivotAreaType enum. Indicates the type of rule being used to describe an area or aspect of the PivotTable
## PivotAreaType enumeration
Indicates the type of rule being used to describe an area or aspect of the PivotTable.
```csharp
public enum PivotAreaType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No Pivot area. |
| Normal | `1` | Represents a header or item. |
| Data | `2` | Represents something in the data area. |
| All | `3` | Represents the whole PivotTable. |
| Origin | `4` | Represents the blank cells at the top-left of the PivotTable (top-right for RTL sheets). |
| Button | `5` | Represents a field button. |
| TopRight | `6` | Represents the blank cells at the top-right of the PivotTable (top-left for RTL sheets). |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
namespace AsposeCellsExamples
{
public class PivotAreaTypeDemo
{
public static void PivotAreaTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apples");
worksheet.Cells["A3"].PutValue("Oranges");
worksheet.Cells["A4"].PutValue("Bananas");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(200);
// Create a PivotTable
int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Add fields to the PivotTable
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
// Create a PivotArea for the PivotTable
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.RuleType = PivotAreaType.Normal;
pivotArea.OnlyData = true;
pivotArea.IsRowGrandIncluded = true;
// Output the PivotArea properties
Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
Console.WriteLine("Only Data: " + pivotArea.OnlyData);
Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);
// Save the workbook
workbook.Save("PivotAreaTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)

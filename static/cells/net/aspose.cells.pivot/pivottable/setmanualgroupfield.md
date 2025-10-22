##PivotTable.SetManualGroupField
PivotTable method. Sets manual field group by the PivotTable
## SetManualGroupField(int, double, double, ArrayList, double) {#setmanualgroupfield_2}
Sets manual field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, double startVal, double endVal,
ArrayList groupByList, double intervalNum)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
using System.Collections;
public class PivotTableMethodSetManualGroupFieldWithInt32DoubleDoubleArrayListDoubDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample numeric data for grouping
worksheet.Cells["A1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(10.5);
worksheet.Cells["A3"].PutValue(15.2);
worksheet.Cells["A4"].PutValue(20.7);
worksheet.Cells["A5"].PutValue(25.1);
worksheet.Cells["A6"].PutValue(30.9);
worksheet.Cells["A7"].PutValue(35.4);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:A7", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
try
{
// Prepare parameters for SetManualGroupField
int baseFieldIndex = 0;
double startVal = 10.0;
double endVal = 40.0;
ArrayList groupByList = new ArrayList() { 10.0 }; // Group by 10s
double intervalNum = 10.0;
// Call SetManualGroupField with numeric parameters
pivotTable.SetManualGroupField(baseFieldIndex, startVal, endVal, groupByList, intervalNum);
// Calculate data to update pivot table
pivotTable.CalculateData();
Console.WriteLine("SetManualGroupField executed successfully with numeric parameters");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetManualGroupField: {ex.Message}");
}
workbook.Save("PivotTableMethodSetManualGroupFieldDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SetManualGroupField(PivotField, double, double, ArrayList, double) {#setmanualgroupfield}
Sets manual field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, double startVal, double endVal,
ArrayList groupByList, double intervalNum)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SetManualGroupField(int, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_3}
Sets manual field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal,
ArrayList groupByList, int intervalNum)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SetManualGroupField(PivotField, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_1}
Sets manual field group by the PivotTable.
```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal,
ArrayList groupByList, int intervalNum)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

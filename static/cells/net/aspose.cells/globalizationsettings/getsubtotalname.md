##GlobalizationSettings.GetSubTotalName
GlobalizationSettings method. Gets the name of PivotFieldSubtotalType type in the PivotTable
## GlobalizationSettings.GetSubTotalName method
Gets the name of [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfSubTotal() method instead.")]
public virtual string GetSubTotalName(PivotFieldSubtotalType subTotalType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type |
### Return Value
The name of [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetSubTotalNameWithPivotFieldSubtotalTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
var globalizationSettings = workbook.Settings.GlobalizationSettings;
PivotFieldSubtotalType subtotalType = PivotFieldSubtotalType.Sum;
string subTotalName = ((CustomGlobalizationSettings)globalizationSettings).GetSubTotalName(subtotalType);
Console.WriteLine($"Subtotal name for {subtotalType}: {subTotalName}");
workbook.Worksheets[0].Cells["A1"].PutValue(subTotalName);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetSubTotalName: {ex.Message}");
}
workbook.Save("GlobalizationSettingsMethodGetSubTotalNameDemo.xlsx");
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetSubTotalName(PivotFieldSubtotalType subTotalType)
{
return $"Custom {subTotalType}";
}
}
}
}
```
### See Also
* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

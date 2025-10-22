##SettablePivotGlobalizationSettings.GetTextOfSubTotal
SettablePivotGlobalizationSettings method. Gets the text of PivotFieldSubtotalType type in the PivotTable
## SettablePivotGlobalizationSettings.GetTextOfSubTotal method
Gets the text of [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.
```csharp
public override string GetTextOfSubTotal(PivotFieldSubtotalType subTotalType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
### Return Value
The text of given type
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class SettablePivotGlobalizationSettingsMethodGetTextOfSubTotalWithPivotFieldSubtotalTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettablePivotGlobalizationSettings
SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();
try
{
// Call GetTextOfSubTotal with different PivotFieldSubtotalType values
string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
string countText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Count);
// Display the results
Console.WriteLine($"Sum subtotal text: {sumText}");
Console.WriteLine($"Average subtotal text: {avgText}");
Console.WriteLine($"Count subtotal text: {countText}");
// Set custom text for subtotals
settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum");
settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Avg");
// Verify the changes
Console.WriteLine($"Modified Sum text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum)}");
Console.WriteLine($"Modified Avg text: {settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTextOfSubTotal method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettablePivotGlobalizationSettingsDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

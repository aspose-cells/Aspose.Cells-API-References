##PivotGlobalizationSettings.GetTextOfProtection
PivotGlobalizationSettings method. Gets the protection name in the PivotTable
## PivotGlobalizationSettings.GetTextOfProtection method
Gets the protection name in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetTextOfProtection()
```
### Return Value
The protection name of PivotTable
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Settings;
namespace AsposeCellsExamples
{
public class PivotGlobalizationSettingsMethodGetTextOfProtectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["B3"].PutValue(2000);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create globalization settings and demonstrate GetTextOfProtection
PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
Console.WriteLine("Protection Text: " + globalizationSettings.GetTextOfProtection());
// Save the workbook
workbook.Save("PivotGlobalizationDemo.xlsx");
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)

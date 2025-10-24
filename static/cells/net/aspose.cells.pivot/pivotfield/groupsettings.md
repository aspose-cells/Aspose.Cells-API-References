##PivotField.GroupSettings
PivotField property. Gets the group settings of the pivot field
## PivotField.GroupSettings property
Gets the group settings of the pivot field.
```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```
### Remarks
If this field is not grouped, Null will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyGroupSettingsDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Access the second base field (assuming it exists)
if (pivotTable.BaseFields.Count > 1)
{
PivotField pivotField = pivotTable.BaseFields[1];
// Check if the field has group settings
if (pivotField.GroupSettings != null)
{
Console.WriteLine("Field has grouping enabled");
Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
}
else
{
Console.WriteLine("Field has no grouping settings");
}
// Example of grouping a numeric field
if (pivotField.GroupSettings == null &&
pivotField.PivotItems.Count > 0 &&
pivotField.PivotItems[0].Value is double)
{
// Group by numeric range (10 unit intervals)
pivotField.GroupBy(10.0, false);
Console.WriteLine("Field grouped by numeric range");
}
}
// Save the modified workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

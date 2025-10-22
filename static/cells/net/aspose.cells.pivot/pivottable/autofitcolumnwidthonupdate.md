##PivotTable.AutofitColumnWidthOnUpdate
PivotTable property. Indicates whether autofitting column width on update
## PivotTable.AutofitColumnWidthOnUpdate property
Indicates whether autofitting column width on update
```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Access the worksheet containing the pivot table
Worksheet worksheet = workbook.Worksheets["PIVOT"];
// Access the pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Disable autofit column width on update
pivotTable.AutofitColumnWidthOnUpdate = false;
// Refresh the pivot table to apply changes
worksheet.RefreshPivotTables();
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

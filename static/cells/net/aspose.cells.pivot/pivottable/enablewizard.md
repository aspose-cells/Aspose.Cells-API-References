##PivotTable.EnableWizard
PivotTable property. Indicates whether the PivotTable Wizard is available
## PivotTable.EnableWizard property
Indicates whether the PivotTable Wizard is available.
```csharp
public bool EnableWizard { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyEnableWizardDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = 1000;
cells["A3"].Value = "Orange";
cells["B3"].Value = 1500;
cells["A4"].Value = "Banana";
cells["B4"].Value = 2000;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Disable the pivot table wizard
pivotTable.EnableWizard = false;
// Save the workbook
workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

##OdsLoadOptions.IsClassicPivotTable
OdsLoadOptions property. Indicates whether the pivot table is classic
## OdsLoadOptions.IsClassicPivotTable property
Indicates whether the pivot table is classic.
```csharp
public bool IsClassicPivotTable { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
{
public static void Run()
{
// Create sample ODS file with pivot table
CreateSampleOdsWithPivotTable();
// Load with IsClassicPivotTable set to true
OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
loadOptionsTrue.IsClassicPivotTable = true;
Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
Console.WriteLine("Loaded with IsClassicPivotTable = true");
Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);
// Load with IsClassicPivotTable set to false
OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
loadOptionsFalse.IsClassicPivotTable = false;
Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
}
private static void CreateSampleOdsWithPivotTable()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate sample data
cells["A1"].Value = "Category";
cells["A2"].Value = "Electronics";
cells["A3"].Value = "Clothing";
cells["A4"].Value = "Books";
cells["B1"].Value = "Sales";
cells["B2"].Value = 1500;
cells["B3"].Value = 800;
cells["B4"].Value = 200;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field (Category)
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field (Sales) and set display name
int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";
// Save as ODS
workbook.Save("SamplePivot.ods", SaveFormat.Ods);
}
}
}
```
### See Also
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

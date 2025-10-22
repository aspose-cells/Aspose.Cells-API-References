##PivotTable.AltTextTitle
PivotTable property. Gets and sets the title of the alter text
## PivotTable.AltTextTitle property
Gets and sets the title of the alter text.
```csharp
public string AltTextTitle { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyAltTextTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["B2"].PutValue("North");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B3"].PutValue("South");
worksheet.Cells["C3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Product C");
worksheet.Cells["B4"].PutValue("East");
worksheet.Cells["C4"].PutValue(3000);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C4", "E3", "SalesPivotTable");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display current AltTextTitle value
Console.WriteLine("Current AltTextTitle value: " + pivotTable.AltTextTitle);
// Set new AltTextTitle value
pivotTable.AltTextTitle = "Sales Data Pivot Table";
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableAltTextTitleDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

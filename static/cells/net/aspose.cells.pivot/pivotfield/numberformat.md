##PivotField.NumberFormat
PivotField property. Represents the custom display format of numbers and dates
## PivotField.NumberFormat property
Represents the custom display format of numbers and dates.
```csharp
public string NumberFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyNumberFormatDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B4"].PutValue(3000);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field with number format
int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[fieldIndex];
dataField.Function = ConsolidationFunction.Sum;
dataField.NumberFormat = "$#,##0.00";
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldNumberFormatDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

##PivotFieldCollection.Item
PivotFieldCollection property. Gets the PivotField Object at the specific index
## PivotFieldCollection indexer (1 of 2)
Gets the PivotField Object at the specific index.
```csharp
public PivotField this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and get the first sheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Access the first row field using Item property and set IsAutoSort
pivotTable.RowFields[0].IsAutoSort = true;
// Save the workbook
workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## PivotFieldCollection indexer (2 of 2)
Gets the PivotField Object of the specific name.
```csharp
public PivotField this[string name] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add sample data for pivot table
ws.Cells["A1"].Value = "Category";
ws.Cells["B1"].Value = "Value";
ws.Cells["A2"].Value = "A";
ws.Cells["B2"].Value = 10;
ws.Cells["A3"].Value = "B";
ws.Cells["B3"].Value = 20;
ws.Cells["A4"].Value = "A";
ws.Cells["B4"].Value = 30;
ws.Cells["A5"].Value = "B";
ws.Cells["B5"].Value = 40;
// Create pivot table
int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pTable = ws.PivotTables[index];
// Add fields to pivot table
pTable.AddFieldToArea(PivotFieldType.Row, "Category");
pTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Demonstrate Item property usage
pTable.DataFields["Sum of Value"].IsAutoSort = true;
pTable.DataFields["Sum of Value"].IsAscendSort = false;
// Refresh and calculate pivot table
pTable.RefreshData();
pTable.CalculateData();
// Save the workbook
wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

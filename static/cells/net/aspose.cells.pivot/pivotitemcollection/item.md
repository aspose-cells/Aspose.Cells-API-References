##PivotItemCollection.Item
PivotItemCollection property. Gets the PivotItem Object at the specific index
## PivotItemCollection indexer (1 of 2)
Gets the PivotItem Object at the specific index.
```csharp
public PivotItem this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = 100;
cells["A3"].Value = "Orange";
cells["B3"].Value = 150;
cells["A4"].Value = "Banana";
cells["B4"].Value = 200;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Access pivot items using Item property
PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
// Demonstrate Item property usage
Console.WriteLine("First pivot item: " + pivotItems[0].Name);
Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
}
}
}
```
### See Also
* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## PivotItemCollection indexer (2 of 2)
Gets the [`PivotItem`](../../pivotitem/) by the specific name.
```csharp
public PivotItem this[string itemValue] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("PivotTest3.xlsx");
// Add a new worksheet for pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];
// Add pivot table
PivotTableCollection pivotTables = pivotSheet.PivotTables;
int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
PivotTable pivotTable = pivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");
// Configure pivot table
pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
pivotTable.ShowColumnGrandTotals = false;
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate Item property usage and move operations
PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
// Access items using Item property
items["4H12"].Move(0, true);
items["DIF400"].Move(-1, true);
pivotTable.CalculateData();
items["CA32"].Move(0, true);
items["AAA3"].Move(-1, true);
// Save the workbook
workbook.Save("PivotItemCollectionDemo_Output.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

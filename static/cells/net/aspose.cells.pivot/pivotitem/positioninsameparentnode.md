##PivotItem.PositionInSameParentNode
PivotItem property. Specifying the position index in the PivotItems under the same parent node
## PivotItem.PositionInSameParentNode property
Specifying the position index in the PivotItems under the same parent node.
```csharp
public int PositionInSameParentNode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyPositionInSameParentNodeDemo
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
PivotField vendorField = pivotTable.RowFields["Vendor"];
vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
pivotTable.ShowColumnGrandTotals = false;
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate PositionInSameParentNode property
PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
// Set positions within same parent node
items["4H12"].PositionInSameParentNode = 1;
items["DIF400"].PositionInSameParentNode = 2;
// Recalculate after changing positions
pivotTable.CalculateData();
// Set positions for another group
items["CA32"].PositionInSameParentNode = 1;
items["AAA3"].PositionInSameParentNode = 2;
// Save the workbook
workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

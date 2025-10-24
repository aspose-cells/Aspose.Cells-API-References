##ListColumn.TotalsCalculation
ListColumn property. Gets and sets the type of calculation in the Totals row of the list column
## ListColumn.TotalsCalculation property
Gets and sets the type of calculation in the Totals row of the list column.
```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnPropertyTotalsCalculationDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item 2");
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["A4"].PutValue("Item 3");
worksheet.Cells["B4"].PutValue(200);
// Create a list object
int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
ListObject listObj = worksheet.ListObjects[listObjIndex];
listObj.ShowTotals = true;
// Set totals calculation for the second column
listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
// Save the workbook
workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
}
}
}
```
### See Also
* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

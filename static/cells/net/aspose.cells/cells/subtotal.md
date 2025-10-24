##Cells.Subtotal
Cells method. Creates subtotals for the range
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}
Creates subtotals for the range.
```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Int32 | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | Int32[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data for subtotaling
CreateSampleData(worksheet);
// Define cell area containing data (A1:C6)
CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);
try
{
// Call Subtotal method with parameters:
// - Group by column 0 (Region)
// - Use SUM function
// - Apply to column 2 (Sales)
worksheet.Cells.Subtotal(
cellArea,
0,
ConsolidationFunction.Sum,
new int[] { 2 }
);
Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
// The ExpandColumnLevel and ExpandRowLevel methods were removed to fix compilation errors
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
}
// Save the result
workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
}
private static void CreateSampleData(Worksheet worksheet)
{
// Create header row
worksheet.Cells["A1"].PutValue("Region");
worksheet.Cells["B1"].PutValue("Product");
worksheet.Cells["C1"].PutValue("Sales");
// Create data rows
object[,] data = new object[,] {
{"North", "Widget", 5000},
{"North", "Gadget", 3000},
{"South", "Widget", 6000},
{"South", "Gadget", 4000},
{"West", "Widget", 4500}
};
// Populate data starting from row 2 (zero-based index 1)
for (int i = 0; i < data.GetLength(0); i++)
{
worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
}
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}
Creates subtotals for the range.
```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList,
bool replace, bool pageBreaks, bool summaryBelowData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Int32 | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | Int32[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | Boolean | Indicates whether replace the current subtotals |
| pageBreaks | Boolean | Indicates whether add page break between groups |
| summaryBelowData | Boolean | Indicates whether add summary below data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data for subtotaling
cells["A1"].PutValue("Category");
cells["B1"].PutValue("Product");
cells["C1"].PutValue("Sales");
object[,] data = new object[,] {
{ "Fruits", "Apple", 1500 },
{ "Fruits", "Orange", 2500 },
{ "Vegetables", "Carrot", 1800 },
{ "Vegetables", "Potato", 3000 },
{ "Fruits", "Banana", 2000 }
};
for (int row = 0; row < 5; row++)
{
for (int col = 0; col < 3; col++)
{
cells[row + 1, col].PutValue(data[row, col]);
}
}
try
{
// Define cell area for subtotal (A1:C6)
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 5;
area.EndColumn = 2;
// Call Subtotal with parameters:
// - Group by first column (0-based index 0)
// - Use Sum function
// - Apply to third column (0-based index 2)
// - Replace existing subtotals, page breaks between groups, summary below data
cells.Subtotal(
area,
0,
ConsolidationFunction.Sum,
new int[] { 2 },
true,
true,
true
);
Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
}
catch (Exception ex)
{
Console.WriteLine($"Error creating subtotal: {ex.Message}");
}
workbook.Save("SubtotalDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

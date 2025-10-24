##AutoFilter.GetCellArea
AutoFilter method. Gets the CellArea where the this AutoFilter applies to
## GetCellArea() {#getcellarea}
Gets the [`CellArea`](../../cellarea/) where the this AutoFilter applies to.
```csharp
public CellArea GetCellArea()
```
### Return Value
the area this filter applies to
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFilterMethodGetCellAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate sample data for AutoFilter demonstration
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Category");
cells["C1"].PutValue("Price");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue("Fruit");
cells["C2"].PutValue(2.5);
cells["A3"].PutValue("Carrot");
cells["B3"].PutValue("Vegetable");
cells["C3"].PutValue(1.2);
cells["A4"].PutValue("Banana");
cells["B4"].PutValue("Fruit");
cells["C4"].PutValue(3.1);
// Apply AutoFilter to headers (row index 0) covering columns A-C (0-2)
AutoFilter autoFilter = worksheet.AutoFilter;
autoFilter.SetRange(0, 0, 2);
try
{
// Get the CellArea where AutoFilter is applied
CellArea result = autoFilter.GetCellArea();
// Output the AutoFilter range coordinates
Console.WriteLine("AutoFilter applied to cell area:");
Console.WriteLine($"Start Row: {result.StartRow}");
Console.WriteLine($"Start Column: {result.StartColumn}");
Console.WriteLine($"End Row: {result.EndRow}");
Console.WriteLine($"End Column: {result.EndColumn}");
// Apply a simple filter to demonstrate functionality (optional)
autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
autoFilter.Refresh();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
}
// Save the workbook with applied AutoFilter
workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetCellArea(bool) {#getcellarea_1}
Gets the [`CellArea`](../../cellarea/) where the specified AutoFilter applies to.
```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```
| Parameter | Type | Description |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Whether refresh the applied range. For the applied range of auto filter, the last row may change when cells data changes. If this flag is true, then the last row of the range will be re-calculated according to current cells data. |
### Return Value
the area this filter applies to
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFilterMethodGetCellAreaWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare sample data for AutoFilter
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
worksheet.Cells["A4"].PutValue("Data3");
// Set AutoFilter range (row 0 to 3, column 0)
worksheet.AutoFilter.SetRange(0, 0, 0);
try
{
// Call GetCellArea with refreshAppliedRange=true
CellArea result = worksheet.AutoFilter.GetCellArea(true);
// Display the AutoFilter's applied range
Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
$"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
$"EndColumn={result.EndColumn}");
Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
}
// Save the modified workbook
workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

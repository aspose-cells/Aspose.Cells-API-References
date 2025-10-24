##Name.GetRange
Name method. Gets the range if this name refers to a range
## GetRange() {#getrange}
Gets the range if this name refers to a range.
```csharp
public Range GetRange()
```
### Return Value
The range.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameMethodGetRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(15);
// Create a named range
int index = workbook.Worksheets.Names.Add("MyRange");
workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
Name namedRange = workbook.Worksheets.Names[index];
// Demonstrate GetRange method
Aspose.Cells.Range range = namedRange.GetRange();
Console.WriteLine("Named Range Address: " + range.Address);
Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
// Modify the range
foreach (Cell cell in range)
{
if (cell.Row == 0)
{
cell.PutValue(cell.StringValue.ToUpper());
}
}
// Save the workbook
workbook.Save("NamedRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetRange(bool) {#getrange_1}
Gets the range if this name refers to a range
```csharp
public Range GetRange(bool recalculate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |
### Return Value
The range.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class NameMethodGetRangeWithBooleanDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Populate sample data
for (int i = 0; i < 4; i++)
{
cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
}
// Create a named range with formula
int nameIndex = wb.Worksheets.Names.Add("testname");
Name name = wb.Worksheets.Names[nameIndex];
name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";
// Use the named range in formulas
cells["C1"].Formula = "=testname";
cells["D1"].Formula = "SUM(testname)";
// Calculate formulas
wb.CalculateFormula();
// Get the range using GetRange(true)
Aspose.Cells.Range namedRange = name.GetRange(true);
Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
$"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");
// Create a chart using the named range
int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("testname", true);
Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetRange(int, int, int) {#getrange_2}
Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.
```csharp
public Range GetRange(int sheetIndex, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The according sheet index. |
| row | Int32 | The according row index. |
| column | Int32 | The according column index |
### Return Value
The range.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameMethodGetRangeWithInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["A4"].PutValue("Dairy");
// Create a named range using the correct method signature
int index = workbook.Worksheets.Names.Add("SubCat");
workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
// Get range using GetRange with row, column and row count parameters
Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
// Display the range reference
Console.WriteLine("Range refers to: " + range.RefersTo);
}
}
}
```
### See Also
* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

##Worksheet.AutoFitRow
Worksheet method. Autofits row height in a rectangle range
## AutoFitRow(int, int, int, int) {#autofitrow_3}
Autofits row height in a rectangle range.
```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
RowCollection rows = worksheet.Cells.Rows;
rows[0].Height = 20;
rows[1].Height = 20;
// Add sample data to cells to demonstrate row autofit
worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
worksheet.Cells["B1"].PutValue("Additional column with text");
worksheet.Cells["A2"].PutValue("Shorter text");
worksheet.Cells["B2"].PutValue("More text");
try
{
Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");
// Call AutoFitRow with parameters: startRow, endRow, startColumn, endColumn
worksheet.AutoFitRow(0, 1, 0, 1);
Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
// Display the effect by showing row heights
Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
}
// Save the result
workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRow(int) {#autofitrow}
Autofits the row height.
```csharp
public void AutoFitRow(int rowIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
### Remarks
AutoFitRow is an imprecise function.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set long text with text wrapping in cell A1
worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
// Auto-fit the first row
worksheet.AutoFitRow(0);
// Save the workbook
workbook.Save("AutoFitRowDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRow(int, int, int) {#autofitrow_1}
Autofits the row height.
```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
### Remarks
This method autofits a row based on content in a range of cells within the row.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells that will affect row height
worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
worksheet.Cells["B2"].PutValue("Additional text in another column");
// AutoFit the row (row 2) between columns 0 and 1 (A to B)
worksheet.AutoFitRow(1, 0, 1);
// Save the workbook
workbook.Save("AutoFitRowDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}
Autofits the row height.
```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitter options |
### Remarks
This method autofits a row based on content in a range of cells within the row.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("This is a test string for autofit");
worksheet.Cells["B1"].PutValue("Another test string in column B");
// Create AutoFitterOptions
AutoFitterOptions options = new AutoFitterOptions
{
AutoFitMergedCells = true,
IgnoreHidden = false,
OnlyAuto = false
};
// Get original row height
double originalHeight = worksheet.Cells.GetRowHeight(0);
Console.WriteLine($"Original row height: {originalHeight}");
// AutoFit the first row
worksheet.AutoFitRow(0, 0, 2, options);
// Get new row height
double newHeight = worksheet.Cells.GetRowHeight(0);
Console.WriteLine($"New row height after AutoFit: {newHeight}");
// Save the workbook
workbook.Save("AutoFitRowExample.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

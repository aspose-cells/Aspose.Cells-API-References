##Worksheet.AutoFitColumns
Worksheet method. Autofits all columns in this worksheet
## AutoFitColumns() {#autofitcolumns}
Autofits all columns in this worksheet.
```csharp
public void AutoFitColumns()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitColumnsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("This is a test string");
worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
worksheet.Cells["C1"].PutValue("Short");
// Auto-fit all columns in the worksheet
worksheet.AutoFitColumns();
// Save the workbook
workbook.Save("AutoFitColumnsDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}
Autofits all columns in this worksheet.
```csharp
public void AutoFitColumns(AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitting options |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
worksheet.Cells["C1"].PutValue(12345.6789);
// Create auto fitter options
AutoFitterOptions options = new AutoFitterOptions();
options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
// Auto fit columns with options
worksheet.AutoFitColumns(options);
// Save the workbook
workbook.Save("AutoFitColumnsWithOptions.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumns(int, int) {#autofitcolumns_2}
Autofits the columns width.
```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
### Remarks
AutoFitColumn is an imprecise function.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to demonstrate autofit
sheet.Cells["A1"].PutValue("Short");
sheet.Cells["B1"].PutValue("Medium length text");
sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
sheet.Cells["D1"].PutValue("Another example with different length");
// AutoFit columns from index 0 to 3
sheet.AutoFitColumns(0, 3);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}
Autofits the columns width.
```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstColumn | Int32 | First column index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |
### Remarks
AutoFitColumn is an imprecise function.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Short text");
worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
worksheet.Cells["C1"].PutValue("Another example with different length");
// Create AutoFitterOptions with specific settings
AutoFitterOptions options = new AutoFitterOptions();
options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
options.IgnoreHidden = false;
options.OnlyAuto = false;
try
{
// Call AutoFitColumns with parameters (firstColumn, lastColumn, options)
worksheet.AutoFitColumns(0, 2, options);
Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
// Display the effect by showing column widths
Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
}
// Save the result
workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}
Autofits the columns width.
```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |
### Remarks
AutoFitColumn is an imprecise function.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data for demonstration
worksheet.Cells["A1"].PutValue("Short");
worksheet.Cells["B1"].PutValue("Medium length text");
worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
// AutoFit columns from column 0 (A) to column 2 (C), with first row 0 and last row 0
worksheet.AutoFitColumns(0, 2, 0, 0);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}
Autofits the columns width.
```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn,
AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row index. |
| firstColumn | Int32 | First column index. |
| lastRow | Int32 | Last row index. |
| lastColumn | Int32 | Last column index. |
| options | AutoFitterOptions | The auto fitting options |
### Remarks
AutoFitColumn is an imprecise function.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with sample data that needs column width adjustment
worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
worksheet.Cells["C1"].PutValue("Short");
worksheet.Cells["A2"].PutValue(12345.6789);
worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
worksheet.Cells["C2"].PutValue(true);
// Create AutoFitterOptions with specific settings
AutoFitterOptions options = new AutoFitterOptions();
options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
options.IgnoreHidden = false;
options.OnlyAuto = false;
try
{
// Call AutoFitColumns with specific parameters (firstRow, firstColumn, lastRow, lastColumn, options)
worksheet.AutoFitColumns(0, 0, 1, 2, options);
Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
// Display column widths after autofit
Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
}
// Save the result
workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

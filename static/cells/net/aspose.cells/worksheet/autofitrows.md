##Worksheet.AutoFitRows
Worksheet method. Autofits all rows in this worksheet
## AutoFitRows() {#autofitrows}
Autofits all rows in this worksheet.
```csharp
public void AutoFitRows()
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
worksheet.Cells["B1"].PutValue("Column B content");
// AutoFit the rows
worksheet.AutoFitRows();
// AutoFit the columns for better visibility
worksheet.AutoFitColumns();
// Save the workbook
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
workbook.Save(outputPath, SaveFormat.Xlsx);
Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRows(bool) {#autofitrows_2}
Autofits all rows in this worksheet.
```csharp
public void AutoFitRows(bool onlyAuto)
```
| Parameter | Type | Description |
| --- | --- | --- |
| onlyAuto | Boolean | True,only autofits the row height when row height is not customed. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowsWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample text to cells to demonstrate row autofit
worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
// AutoFit rows with auto-merge consideration
worksheet.AutoFitRows(true);
// Save the workbook
workbook.Save("AutoFitRowsDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}
Autofits all rows in this worksheet.
```csharp
public void AutoFitRows(AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | AutoFitterOptions | The auto fitter options |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and formatting
worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
// Merge cells to demonstrate merged cell auto-fitting
worksheet.Cells.Merge(3, 0, 2, 1);
worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");
// AutoFit rows with specific options
worksheet.AutoFitRows(new AutoFitterOptions
{
AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
MaxRowHeight = 100,  // Set reasonable max height
OnlyAuto = true
});
// Save the workbook
workbook.Save("AutoFitRowsDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRows(int, int) {#autofitrows_3}
Autofits row height in a range.
```csharp
public void AutoFitRows(int startRow, int endRow)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Populate cells with sample data and styles
for (int i = 0; i <= 8; i++)
{
Cell cell = cells[i, i];
cell.Value = "Sample text for row " + i;
if (i % 2 == 0)
{
Style style = cell.GetStyle();
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
cell.SetStyle(style);
}
}
// Auto-fit rows from index 0 to 8
sheet.AutoFitRows(0, 8);
// Output the resulting row heights
for (int i = 0; i <= 8; i++)
{
Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
}
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}
Autofits row height in a range.
```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| endRow | Int32 | End row index. |
| options | AutoFitterOptions | The options of auto fitter. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
// Create auto fitter options
AutoFitterOptions options = new AutoFitterOptions();
options.OnlyAuto = true;
// Auto fit rows 0 to 1 with options
worksheet.AutoFitRows(0, 1, options);
// Save the workbook
workbook.Save("AutoFitRowsDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

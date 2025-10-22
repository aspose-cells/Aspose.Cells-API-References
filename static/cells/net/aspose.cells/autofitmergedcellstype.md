##Enum AutoFitMergedCellsType
Aspose.Cells.AutoFitMergedCellsType enum. Represents the type of auto fitting merged cells
## AutoFitMergedCellsType enumeration
Represents the type of auto fitting merged cells.
```csharp
public enum AutoFitMergedCellsType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Ignore merged cells. |
| FirstLine | `1` | Only expands the height of the first row. |
| LastLine | `2` | Only expands the height of the last row. |
| EachLine | `3` | Expands the height of each row. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
public class AutoFitMergedCellsTypeDemo
{
public static void AutoFitMergedCellsTypeExample()
{
//Instantiating an Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the newly added worksheet
Worksheet sheet1 = workbook.Worksheets[0];
// Create a range A1:B2
Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);
// Merge the cells
range.Merge();
// Insert value to the merged cell A1
sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";
// Create a style object
Style style = sheet1.Cells[0, 0].GetStyle();
// Set wrapping text on
style.IsTextWrapped = true;
// Apply the style to the cell
sheet1.Cells[0, 0].SetStyle(style);
// Create an object for AutoFitterOptions
AutoFitterOptions options = new AutoFitterOptions();
// Only expands the height of the first row.
options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;
// Autofit rows in the sheet(including the merged cells)
sheet1.AutoFitRows(options);
int index = workbook.Worksheets.Add();
Worksheet sheet2 = workbook.Worksheets[index];
sheet2.Name = "Sheet2";
// Create a range A1:B2
Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);
// Merge the cells
range2.Merge();
// Insert value to the merged cell A1
sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";
// Create a style object
Style style2 = sheet2.Cells[0, 0].GetStyle();
// Set wrapping text on
style2.IsTextWrapped = true;
// Apply the style to the cell
sheet2.Cells[0, 0].SetStyle(style);
// Create an object for AutoFitterOptions
AutoFitterOptions options2 = new AutoFitterOptions();
// Only expands the height of the last row.
options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;
// Autofit rows in the sheet(including the merged cells)
sheet2.AutoFitRows(options2);
index = workbook.Worksheets.Add();
Worksheet sheet3 = workbook.Worksheets[index];
sheet3.Name = "Sheet3";
// Create a range A1:B2
Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);
// Merge the cells
range3.Merge();
// Insert value to the merged cell A1
sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";
// Create a style object
Style style3 = sheet3.Cells[0, 0].GetStyle();
// Set wrapping text on
style3.IsTextWrapped = true;
// Apply the style to the cell
sheet3.Cells[0, 0].SetStyle(style);
// Create an object for AutoFitterOptions
AutoFitterOptions options3 = new AutoFitterOptions();
// Only expands the height of each row.
options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
// Autofit rows in the sheet(including the merged cells)
sheet3.AutoFitRows(options3);
index = workbook.Worksheets.Add();
Worksheet sheet4 = workbook.Worksheets[index];
sheet4.Name = "Sheet4";
// Create a range A1:B2
Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);
// Merge the cells
range4.Merge();
// Insert value to the merged cell A1
sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";
// Create a style object
Style style4 = sheet4.Cells[0, 0].GetStyle();
// Set wrapping text on
style4.IsTextWrapped = true;
// Apply the style to the cell
sheet4.Cells[0, 0].SetStyle(style);
// Create an object for AutoFitterOptions
AutoFitterOptions options4 = new AutoFitterOptions();
// Ignore merged cells.
options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;
// Autofit rows in the sheet(not including the merged cells)
sheet4.AutoFitRows(options4);
// Save the workbook
workbook.Save("AutoFitMergedCellsTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

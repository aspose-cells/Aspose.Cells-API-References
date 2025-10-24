##Cell.SetStyle
Cell method. Sets the cell style
## SetStyle(Style) {#setstyle}
Sets the cell style.
```csharp
public void SetStyle(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
### Remarks
If the border settings are changed, the border of adjust cells will be updated too.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetStyleWithStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style and set its properties
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.Yellow;
// Apply the style to cell B2 (1,1 in zero-based index)
cells[1, 1].SetStyle(style);
// Save the workbook
workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetStyle(Style, bool) {#setstyle_2}
Apply the changed property of style to the cell.
```csharp
public void SetStyle(Style style, bool explicitFlag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetStyleWithStyleBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create styles directly
Style style1 = workbook.CreateStyle();
style1.Name = "MyStyle1";
style1.Font.Name = "Arial";
style1.Font.Size = 12;
style1.Font.IsBold = true;
Style style2 = workbook.CreateStyle();
style2.Name = "MyStyle2";
style2.Font.Name = "Times New Roman";
style2.Font.Size = 14;
style2.Font.Color = System.Drawing.Color.Red;
// Apply styles to cells with the SetStyle method
Cell cell1 = worksheet.Cells["A1"];
cell1.PutValue("Styled Text 1");
cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue("Styled Text 2");
cell2.SetStyle(style2, false); // false to overwrite all style elements
// Save the workbook
workbook.Save("SetStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetStyle(Style, StyleFlag) {#setstyle_1}
Apply the cell style based on flags.
```csharp
public void SetStyle(Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| flag | StyleFlag | The style flag. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellMethodSetStyleWithStyleStyleFlagDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a style and set its properties
Style style = workbook.CreateStyle();
style.Font.Color = Color.Red;
style.Name = "CustomStyle";
// Create a style flag and set it to apply all formatting
StyleFlag flag = new StyleFlag();
flag.All = true;
// Get cells and set value to A1
Cells cells = sheet.Cells;
Cell cell = cells["A1"];
cell.PutValue("Sample Text");
// Apply the style to the cell using SetStyle
cell.SetStyle(style, flag);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

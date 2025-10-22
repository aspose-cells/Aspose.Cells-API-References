##Workbook.CreateStyle
Workbook method. Creates a new style
## CreateStyle() {#createstyle}
Creates a new style.
```csharp
public Style CreateStyle()
```
### Return Value
Returns a style object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCreateStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a new style using CreateStyle method
Style newStyle = workbook.CreateStyle();
// Set style properties
newStyle.Font.Name = "Arial";
newStyle.Font.Size = 12;
newStyle.Font.IsBold = true;
newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
newStyle.Pattern = BackgroundType.Solid;
newStyle.IsTextWrapped = true;
// Create style flag and set flags
StyleFlag flag = new StyleFlag();
flag.FontName = true;
flag.FontSize = true;
flag.FontBold = true;
flag.CellShading = true;
flag.WrapText = true;
// Apply the style to cell A1
Cell cell = worksheet.Cells["A1"];
cell.PutValue("This text has a custom style with wrapping");
worksheet.Cells.ApplyStyle(newStyle, flag);
// Auto-fit the column
worksheet.AutoFitColumn(0);
// Save the workbook
workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## CreateStyle(bool) {#createstyle_1}
Creates a new style.
```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Incidates whether clones the default style |
### Return Value
Returns a style object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCreateStyleWithBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook wb = new Workbook();
// Access first worksheet
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Create a new style (false = don't inherit from default style)
Style style = wb.CreateStyle(false);
style.Font.Color = System.Drawing.Color.Blue;
style.Font.IsBold = true;
// Apply the style to a cell
Cell cell = cells["A1"];
cell.SetStyle(style);
cell.PutValue("Styled Text");
// Save the workbook
wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

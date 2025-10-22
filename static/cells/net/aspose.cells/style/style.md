##Style.Style
Style constructor. Initializes a new instance of the Style class
## Style constructor
Initializes a new instance of the [`Style`](../) class.
```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```
### Remarks
NOTE: This constructor is now obsolete. Instead, please use CellsFactory.CreateStyle() method. This property will be removed 6 months later since October 2016. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style using the constructor
Style style = new Style();
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Red;
style.Pattern = BackgroundType.Solid;
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Styled Text");
cell.SetStyle(style);
// Save the workbook
workbook.Save("StyleConstructorDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

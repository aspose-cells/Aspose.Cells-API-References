##Row.CopySettings
Row method. Copy settings of row such as style height visibility ...etc
## Row.CopySettings method
Copy settings of row, such as style, height, visibility, ...etc.
```csharp
public void CopySettings(Row source, bool checkStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Row | the source row whose settings will be copied to this one |
| checkStyle | Boolean | whether check and gather style. Only takes effect and be needed when two row objects belong to different workbook and the styles of two workbooks are different. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RowMethodCopySettingsWithRowBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and style source row
Row sourceRow = worksheet.Cells.Rows[0];
Style sourceStyle = workbook.CreateStyle();
sourceStyle.BackgroundColor = Color.Blue;
sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
sourceRow.Height = 25;
sourceRow.IsHidden = false;
// Create target row
Row targetRow = worksheet.Cells.Rows[1];
// Demonstrate CopySettings with copyStyle=true
targetRow.CopySettings(sourceRow, true);
// Verify settings were copied
Console.WriteLine($"Target row height: {targetRow.Height}");
Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");
workbook.Save("RowCopySettingsDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

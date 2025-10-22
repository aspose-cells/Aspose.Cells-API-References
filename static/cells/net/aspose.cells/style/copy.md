##Style.Copy
Style method. Copies data from another style object
## Style.Copy method
Copies data from another style object
```csharp
public void Copy(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | Source Style object |
### Remarks
This method does not copy the name of the style. If you want to copy the name, please call the following codes after copying style: destStyle.Name = style.Name.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodCopyWithStyleDemo
{
public static void Run()
{
// Create source workbook with sample data
Workbook srcWorkbook = new Workbook();
Worksheet srcSheet = srcWorkbook.Worksheets[0];
srcSheet.Cells["A1"].PutValue("Sample Text");
Style srcStyle = srcWorkbook.CreateStyle();
srcStyle.Font.Name = "Arial";
srcStyle.Font.Size = 14;
srcSheet.Cells["A1"].SetStyle(srcStyle);
// Create destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Copy the style from source to destination
Style destStyle = destWorkbook.CreateStyle();
destStyle.Copy(srcStyle);
// Apply the copied style
destSheet.Cells["B2"].PutValue("Copied Style Text");
destSheet.Cells["B2"].SetStyle(destStyle);
// Save the result
destWorkbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

##Row.IsHeightMatched
Row property. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is automatic without custom height value set by user
## Row.IsHeightMatched property
Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.
```csharp
public bool IsHeightMatched { get; set; }
```
### Remarks
When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [`AutoFitRows`](../../worksheet/autofitrows/)) to get the same result with what is shown in ms excel when you opening the workbook in it.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyIsHeightMatchedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and style to demonstrate row height matching
worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
worksheet.Cells["B1"].PutValue("Another cell in the same row");
// Apply word wrap to force height adjustment
Style style = worksheet.Cells["A1"].GetStyle();
style.IsTextWrapped = true;
worksheet.Cells["A1"].SetStyle(style);
// Auto-fit the row to match content height
worksheet.AutoFitRow(0);
// Check if row height matches its content
Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

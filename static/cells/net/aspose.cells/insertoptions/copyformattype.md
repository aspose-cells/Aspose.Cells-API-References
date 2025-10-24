##InsertOptions.CopyFormatType
InsertOptions property.
## InsertOptions.CopyFormatType property
```csharp
public CopyFormatType CopyFormatType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class InsertOptionsPropertyCopyFormatTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values and formatting for demonstration
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["A3"].PutValue("Item2");
// Create InsertOptions and set CopyFormatType
InsertOptions options = new InsertOptions();
options.CopyFormatType = CopyFormatType.SameAsAbove;
// Insert row with formatting from above
worksheet.Cells.InsertRows(2, 1, options);
// Save the result
workbook.Save("InsertWithFormatting.xlsx");
}
}
}
```
### See Also
* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

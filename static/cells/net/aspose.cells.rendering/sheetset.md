##Class SheetSet
Aspose.Cells.Rendering.SheetSet class. Describes a set of sheets
## SheetSet class
Describes a set of sheets.
```csharp
public class SheetSet
```
## Constructors
| Name | Description |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Creates a sheet set based on exact sheet indexes. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Creates a sheet set based on exact sheet names. |
## Properties
| Name | Description |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Gets a set with active sheet of the workbook. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Gets a set with all sheets of the workbook in their original order. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Gets a set with visible sheets of the workbook in their original order. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SheetSetDemo
{
public static void SheetSetExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(456);
worksheet = workbook.Worksheets.Add("test1");
worksheet.Cells["A1"].PutValue("test Data");
worksheet.Cells["A2"].PutValue(234);
worksheet.Cells["A3"].PutValue(333);
worksheet.IsVisible = false;
worksheet = workbook.Worksheets.Add("test2");
worksheet.Cells["A1"].PutValue("test Data222");
worksheet.Cells["A2"].PutValue(234444);
worksheet.Cells["A3"].PutValue(333555);
workbook.Worksheets.ActiveSheetIndex = 0;
// Create a PdfSaveOptions object
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Set the SheetSet property to include only the active sheet
pdfSaveOptions.SheetSet = SheetSet.Active;
// Save the workbook to a PDF file
workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);
// Set the SheetSet property to include all visible sheets
pdfSaveOptions.SheetSet = SheetSet.Visible;
// Save the workbook to a PDF file
workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);
// Set the SheetSet property to include all sheets
pdfSaveOptions.SheetSet = SheetSet.All;
// Save the workbook to a PDF file
workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)

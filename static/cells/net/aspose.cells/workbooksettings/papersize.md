##WorkbookSettings.PaperSize
WorkbookSettings property. Gets and sets the default print paper size
## WorkbookSettings.PaperSize property
Gets and sets the default print paper size.
```csharp
public PaperSizeType PaperSize { get; set; }
```
### Remarks
If there is no setting about paper size,MS Excel will use default printer's setting.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyPaperSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set paper size to A5
workbook.Settings.PaperSize = PaperSizeType.PaperA5;
// Verify the paper size is set correctly in the first worksheet
Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

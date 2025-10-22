##LoadOptions.SetPaperSize
LoadOptions method. Sets the default print paper size from default printers setting
## LoadOptions.SetPaperSize method
Sets the default print paper size from default printer's setting.
```csharp
public void SetPaperSize(PaperSizeType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | PaperSizeType | The default paper size. |
### Remarks
If there is no setting about paper size,MS Excel will use default printer's setting.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
{
public static void Run()
{
// Create load options and set paper size to A5
LoadOptions options = new LoadOptions();
options.SetPaperSize(PaperSizeType.PaperA5);
// Load workbook with the specified options
Workbook workbook = new Workbook("example.xlsx", options);
// Verify the paper size is set correctly
Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
}
}
}
```
### See Also
* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

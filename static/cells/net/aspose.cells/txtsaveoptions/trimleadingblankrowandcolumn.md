##TxtSaveOptions.TrimLeadingBlankRowAndColumn
TxtSaveOptions property. Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property
Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.
```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```
### Remarks
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [`LightCellsDataProvider`](../lightcellsdataprovider/) or by speicifing [`ExportArea`](../exportarea/)
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
{
public static void Run()
{
// Create a sample workbook with some data and blank rows/columns
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data with leading blank rows and columns
worksheet.Cells["C3"].PutValue("Data1");
worksheet.Cells["D4"].PutValue("Data2");
worksheet.Cells["E5"].PutValue("Data3");
// Save without trimming leading blanks
TxtSaveOptions saveOptions = new TxtSaveOptions();
saveOptions.TrimLeadingBlankRowAndColumn = false;
workbook.Save("output_with_blanks.csv", saveOptions);
// Save with trimming leading blanks
saveOptions.TrimLeadingBlankRowAndColumn = true;
workbook.Save("output_trimmed.csv", saveOptions);
Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

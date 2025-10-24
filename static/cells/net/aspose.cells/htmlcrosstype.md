##Enum HtmlCrossType
Aspose.Cells.HtmlCrossType enum. Represents five types of html cross string
## HtmlCrossType enumeration
Represents five types of html cross string.
```csharp
public enum HtmlCrossType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated |
| MSExport | `1` | Display the string like MS Excel exporting html. |
| Cross | `2` | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | `3` | Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | `4` | Only displaying the string within the width of cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassHtmlCrossTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample");
worksheet.Cells["B1"].PutValue("Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["B2"].PutValue(456);
// Create HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
// Set cross type to MSExport
options.HtmlCrossStringType = HtmlCrossType.MSExport;
// Save workbook with HTML options
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

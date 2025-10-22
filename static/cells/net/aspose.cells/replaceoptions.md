##Class ReplaceOptions
Aspose.Cells.ReplaceOptions class. Represent the replace options
## ReplaceOptions class
Represent the replace options.
```csharp
public class ReplaceOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Indicates if the searched string is case sensitive. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | The rich formatted settings for the replaced text. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Indicates whether to match entire cells contents |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Indicates whether the searched key is regex. If true then the searched key will be taken as regex. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Gets and sets flags of applying font settings. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ReplaceOptionsDemo
{
public static void ReplaceOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
sheet.Cells["A1"].PutValue("Hello World");
sheet.Cells["A2"].PutValue("Hello Aspose");
sheet.Cells["A3"].PutValue("Goodbye World");
// Create ReplaceOptions
ReplaceOptions options = new ReplaceOptions
{
CaseSensitive = false,
MatchEntireCellContents = false,
RegexKey = false
};
// Replace "Hello" with "Hi" in the worksheet
int replacedCount = workbook.Replace("Hello", "Hi", options);
// Output the number of replacements made
Console.WriteLine($"Number of replacements made: {replacedCount}");
// Save the workbook
workbook.Save("ReplaceOptionsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)

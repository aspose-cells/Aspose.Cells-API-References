##ReplaceOptions.RegexKey
ReplaceOptions property. Indicates whether the searched key is regex. If true then the searched key will be taken as regex
## ReplaceOptions.RegexKey property
Indicates whether the searched key is regex. If true then the searched key will be taken as regex.
```csharp
public bool RegexKey { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReplaceOptionsPropertyRegexKeyDemo
{
public static void Run()
{
// Create workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("apple");
worksheet.Cells["A2"].PutValue("banana");
worksheet.Cells["A3"].PutValue("orange");
worksheet.Cells["A4"].PutValue("pear");
worksheet.Cells["A5"].PutValue("plum");
// Create replace options with regex
ReplaceOptions options = new ReplaceOptions();
options.RegexKey = true; // Enable regex matching
// Replace all words starting with 'p' or 'b' followed by a vowel
string pattern = "^[pb][aeiou]";
string replacement = "FRUIT";
// Perform the replacement
workbook.Replace(pattern, replacement, options);
// Save the result
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

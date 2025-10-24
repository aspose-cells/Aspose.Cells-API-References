##Cell.Replace
Cell method. Replace text of the cell with options
## Cell.Replace method
Replace text of the cell with options.
```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| placeHolder | String | Cell placeholder |
| newValue | String | String value to replace |
| options | ReplaceOptions | The replace options |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodReplaceWithStringStringReplaceOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello World");
worksheet.Cells["A2"].PutValue("hello world");
worksheet.Cells["A3"].PutValue("HELLO WORLD");
worksheet.Cells["B1"].PutValue("Replaced");
// Create replace options
ReplaceOptions options = new ReplaceOptions();
options.CaseSensitive = false;
options.MatchEntireCellContents = false;
// Get font settings from cell B1 to apply to replacements
options.FontSettings = worksheet.Cells["B1"].GetCharacters();
// Replace all variations of "hello" with "Hi" using the options
foreach (Cell cell in worksheet.Cells)
{
cell.Replace("Hello", "Hi", options);
}
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

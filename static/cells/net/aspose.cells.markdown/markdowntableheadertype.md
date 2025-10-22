##Enum MarkdownTableHeaderType
Aspose.Cells.Markdown.MarkdownTableHeaderType enum. Represents the header type of the table in the markdown file
## MarkdownTableHeaderType enumeration
Represents the header type of the table in the markdown file.
```csharp
public enum MarkdownTableHeaderType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| FirstRow | `0` | First row as header of the table. |
| ColumnHeader | `1` | Column name (such as A,B,C...) as header of the table. |
| Empty | `2` | An empty header row. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;
namespace AsposeCellsExamples
{
public class MarkdownClassMarkdownTableHeaderTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
// Set Markdown save options
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
// Save as Markdown file
workbook.Save("output.md", saveOptions);
// Verify the output
string text = File.ReadAllText("output.md");
Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)

##MarkdownSaveOptions.TableHeaderType
MarkdownSaveOptions property. Gets and sets how set the header of the table
## MarkdownSaveOptions.TableHeaderType property
Gets and sets how set the header of the table.
```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsPropertyTableHeaderTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
// Create MarkdownSaveOptions and set TableHeaderType
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
// Save as markdown with specified options
workbook.Save("output.md", saveOptions);
}
}
}
```
### See Also
* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

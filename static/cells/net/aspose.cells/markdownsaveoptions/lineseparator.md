##MarkdownSaveOptions.LineSeparator
MarkdownSaveOptions property. Gets and sets the line separator
## MarkdownSaveOptions.LineSeparator property
Gets and sets the line separator.
```csharp
public string LineSeparator { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsPropertyLineSeparatorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Value1");
worksheet.Cells["B2"].PutValue("Value2");
// Configure Markdown save options with custom line separator
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
{
LineSeparator = "\n", // Using Unix-style line endings
Encoding = Encoding.UTF8
};
// Save as Markdown file
workbook.Save("MarkdownWithLineSeparator.md", saveOptions);
Console.WriteLine("Markdown file saved with custom line separator.");
}
}
}
```
### See Also
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

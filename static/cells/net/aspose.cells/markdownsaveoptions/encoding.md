##MarkdownSaveOptions.Encoding
MarkdownSaveOptions property. Gets and sets the default encoding
## MarkdownSaveOptions.Encoding property
Gets and sets the default encoding.
```csharp
public Encoding Encoding { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsPropertyEncodingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample");
worksheet.Cells["B1"].PutValue("Markdown");
// Configure save options with UTF8 encoding
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
{
Encoding = Encoding.UTF8
};
// Save with specified encoding
workbook.Save("MarkdownWithEncoding.md", saveOptions);
Console.WriteLine("Markdown file saved with UTF-8 encoding.");
}
}
}
```
### See Also
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

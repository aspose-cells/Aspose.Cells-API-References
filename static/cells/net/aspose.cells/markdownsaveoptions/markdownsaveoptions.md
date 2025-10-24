##MarkdownSaveOptions.MarkdownSaveOptions
MarkdownSaveOptions constructor. Creates options for saving markdown document
## MarkdownSaveOptions constructor
Creates options for saving markdown document
```csharp
public MarkdownSaveOptions()
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MarkdownSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
// Demonstrate MarkdownSaveOptions constructor
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
{
Encoding = Encoding.UTF8,
FormatStrategy = CellValueFormatStrategy.DisplayString,
LineSeparator = Environment.NewLine
};
// Save as Markdown
workbook.Save("MarkdownOutput.md", saveOptions);
Console.WriteLine("Markdown file created successfully.");
}
}
}
```
### See Also
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

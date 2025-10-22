##HtmlSaveOptions.CssStyles
HtmlSaveOptions property. Gets or sets the additional css styles for the formatter. Only works when SaveAsSingleFile is True.  CssStylesbody  padding 5px
## HtmlSaveOptions.CssStyles property
Gets or sets the additional css styles for the formatter. Only works when [`SaveAsSingleFile`](../saveassinglefile/) is True.  CssStyles="body { padding: 5px }";
```csharp
public string CssStyles { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyCssStylesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set custom CSS styles
saveOptions.CssStyles = @"
body {
font-family: Arial;
background-color: #f0f0f0;
}
table {
border-collapse: collapse;
width: 100%;
}
td {
border: 1px solid #ddd;
padding: 8px;
}";
// Save the workbook with custom CSS styles
workbook.Save("HtmlWithCustomStyles.html", saveOptions);
Console.WriteLine("HTML file with custom CSS styles created successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

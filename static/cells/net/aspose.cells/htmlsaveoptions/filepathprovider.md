##HtmlSaveOptions.FilePathProvider
HtmlSaveOptions property. Gets or sets the IFilePathProvider for exporting Worksheet to html separately
## HtmlSaveOptions.FilePathProvider property
Gets or sets the IFilePathProvider for exporting Worksheet to html separately.
```csharp
public IFilePathProvider FilePathProvider { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyFilePathProviderDemo
{
public static void Run()
{
// Create a new workbook and add some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
// Create HtmlSaveOptions and set the FilePathProvider
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.FilePathProvider = new CustomFilePathProvider();
// Save the workbook to HTML format
workbook.Save("output.html", saveOptions);
Console.WriteLine("Workbook saved to HTML with custom file paths.");
}
}
public class CustomFilePathProvider : IFilePathProvider
{
public string GetFullName(string sheetName)
{
// Custom logic to generate file paths
return $"custom_{sheetName}";
}
}
}
```
### See Also
* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

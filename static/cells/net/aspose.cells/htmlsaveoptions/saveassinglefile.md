##HtmlSaveOptions.SaveAsSingleFile
HtmlSaveOptions property. Indicates whether save the html as single file. The default value is false
## HtmlSaveOptions.SaveAsSingleFile property
Indicates whether save the html as single file. The default value is false.
```csharp
public bool SaveAsSingleFile { get; set; }
```
### Remarks
If there are multiple worksheets or other required resources such as pictures in the workbook, commonly those worksheets and other resources need to be saved into separate files. For some scenarios, user maybe need to get only one resultant file such as for the convenience of transferring. If so, user may set this property as true.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Export");
// Initialize HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.SaveAsSingleFile = true;
saveOptions.ExportPageHeaders = true;
// Save the workbook as single HTML file
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
// Verify the output file exists
if (File.Exists(outputPath))
{
Console.WriteLine("HTML saved as single file successfully.");
}
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

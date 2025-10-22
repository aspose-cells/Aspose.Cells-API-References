##XlsSaveOptions.IsTemplate
XlsSaveOptions property. Indicates whether saving a template file
## XlsSaveOptions.IsTemplate property
Indicates whether saving a template file.
```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with corresponding save format(xlt for true and xls for false). This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsSaveOptionsPropertyIsTemplateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Template");
// Save as template file
string outputPath = "output_template.xlt";
XlsSaveOptions saveOptions = new XlsSaveOptions();
saveOptions.IsTemplate = true;
using (FileStream fs = File.Create(outputPath))
{
workbook.Save(fs, saveOptions);
}
// Verify the saved file format
Workbook loadedWorkbook = new Workbook(outputPath);
Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
}
}
}
```
### See Also
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

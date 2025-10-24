##SaveOptions.CreateDirectory
SaveOptions property. If true and the directory does not exist the directory will be automatically created before saving the file
## SaveOptions.CreateDirectory property
If true and the directory does not exist, the directory will be automatically created before saving the file.
```csharp
public bool CreateDirectory { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyCreateDirectoryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Set save options with CreateDirectory enabled
XlsSaveOptions saveOptions = new XlsSaveOptions();
saveOptions.CreateDirectory = true;
// Save the workbook to a new directory (will be created automatically)
string outputPath = "OutputDirectory/example.xls";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("File saved successfully with directory creation.");
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

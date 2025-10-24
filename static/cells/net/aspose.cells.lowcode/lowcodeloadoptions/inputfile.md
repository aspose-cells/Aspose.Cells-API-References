##LowCodeLoadOptions.InputFile
LowCodeLoadOptions property. Gets and sets the filewith path if needed of the template
## LowCodeLoadOptions.InputFile property
Gets and sets the file(with path if needed) of the template.
```csharp
public string InputFile { get; set; }
```
### Remarks
When setting a non-null and non-empty path to this property, the previously set value for [`InputStream`](../inputstream/) will be ignored.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeLoadOptionsPropertyInputFileDemo
{
public static void Run()
{
// Create and save a sample template file
Workbook templateWorkbook = new Workbook();
templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
const string templatePath = "LowCodeTemplate.xlsx";
templateWorkbook.Save(templatePath);
// Initialize LowCodeLoadOptions and demonstrate InputFile property
LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);
// Set InputFile property to use our template
loadOptions.InputFile = templatePath;
Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);
// Load workbook using the specified template file
Workbook workbook = new Workbook(loadOptions.InputFile);
// Modify the loaded template
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);
// Save the modified workbook
workbook.Save("PropertyInputFileDemo_Output.xlsx");
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

##JsonSaveOptions.AlwaysExportAsJsonObject
JsonSaveOptions property. Indicates whether always exporting excel to json as object even there is only a worksheet in the file
## JsonSaveOptions.AlwaysExportAsJsonObject property
Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.
```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
{
public static void Run()
{
// Create a sample workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Set some sample data in first worksheet
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Value");
cells["A2"].PutValue("Item1");
cells["B2"].PutValue(100);
// Configure JSON save options
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.AlwaysExportAsJsonObject = true;
saveOptions.ExportNestedStructure = true;
saveOptions.SkipEmptyRows = true;
// Save to JSON file
string outputPath = "output.json";
workbook.Save(outputPath, saveOptions);
// Display the saved JSON content
string jsonContent = File.ReadAllText(outputPath);
Console.WriteLine(jsonContent);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

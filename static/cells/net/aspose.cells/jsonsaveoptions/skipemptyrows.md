##JsonSaveOptions.SkipEmptyRows
JsonSaveOptions property. Indicates whether skipping emtpy rows
## JsonSaveOptions.SkipEmptyRows property
Indicates whether skipping emtpy rows.
```csharp
public bool SkipEmptyRows { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertySkipEmptyRowsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Sample data - add some cells with values and leave some rows empty
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
// Leave row 3 empty
worksheet.Cells["A4"].PutValue("Data3");
worksheet.Cells["B4"].PutValue("Data4");
// Configure JSON save options with SkipEmptyRows
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
// Save to JSON
string outputPath = "output.json";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

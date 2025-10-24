##JsonSaveOptions.ExportNestedStructure
JsonSaveOptions property. Exported as parentchild hierarchy Json structure
## JsonSaveOptions.ExportNestedStructure property
Exported as parent-child hierarchy Json structure.
```csharp
public bool ExportNestedStructure { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyExportNestedStructureDemo
{
public static void Run()
{
// Create a sample workbook with nested data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create nested data structure
worksheet.Cells["A1"].PutValue("Parent");
worksheet.Cells["B1"].PutValue("Child");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["B2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Fruits");
worksheet.Cells["B3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Vegetables");
worksheet.Cells["B4"].PutValue("Carrot");
// Configure JSON save options with ExportNestedStructure
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.ExportNestedStructure = true;
saveOptions.AlwaysExportAsJsonObject = true;
// Save with nested structure
string outputPath = "output_nested.json";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

##JsonSaveOptions.ExportAsString
JsonSaveOptions property. Exports the string value of the cells to json
## JsonSaveOptions.ExportAsString property
Exports the string value of the cells to json.
```csharp
public bool ExportAsString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonSaveOptionsPropertyExportAsStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create sample data with numeric values
cells["A1"].PutValue("Age");
cells["B1"].PutValue("Score");
cells["A2"].PutValue(30);
cells["B2"].PutValue(95.5);
JsonSaveOptions exportOptions = new JsonSaveOptions();
exportOptions.ExportAsString = true;
string jsonOutput = JsonUtility.ExportRangeToJson(cells.CreateRange("A1:B2"), exportOptions);
Console.WriteLine("Exported JSON with ExportAsString=true:\n" + jsonOutput);
}
}
}
```
### See Also
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

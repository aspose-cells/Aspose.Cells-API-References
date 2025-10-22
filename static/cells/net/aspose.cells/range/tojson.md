##Range.ToJson
Range method. Convert the range to JSON value
## Range.ToJson method
Convert the range to JSON value.
```csharp
public string ToJson(JsonSaveOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | JsonSaveOptions | The options of converting |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodToJsonWithJsonSaveOptionsDemo
{
public static void Run()
{
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
// Sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["B1"].PutValue("Age");
sheet.Cells["A2"].PutValue("John");
sheet.Cells["B2"].PutValue(30);
Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:B2");
JsonSaveOptions saveOptions = new JsonSaveOptions();
saveOptions.AlwaysExportAsJsonObject = true;
saveOptions.ToExcelStruct = true;
string json = range.ToJson(saveOptions);
Console.WriteLine(json);
}
}
}
```
### See Also
* class [JsonSaveOptions](../../jsonsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

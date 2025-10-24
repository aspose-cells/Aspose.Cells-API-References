##JsonUtility.ExportRangeToJson
JsonUtility method. Exporting the range to json file
## ExportRangeToJson(Range, ExportRangeToJsonOptions) {#exportrangetojson_1}
Exporting the range to json file.
```csharp
[Obsolete("Use ExportRangeToJson(Range range, JsonSaveOptions options) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ExportRangeToJson(Range range, ExportRangeToJsonOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | ExportRangeToJsonOptions | The options of exporting. |
### Return Value
The json string value.
### Remarks
NOTE: This member is now obsolete. Instead, please use ExportRangeToJson(Range range, JsonSaveOptions options) method. This property will be removed 6 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonUtilityMethodExportRangeToJsonWithRangeExportRangeToJsonOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a range covering the data
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
// Create export options
ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
options.ExportAsString = true;
// Export range to JSON
string json = JsonUtility.ExportRangeToJson(range, options);
Console.WriteLine(json);
}
}
}
```
### See Also
* class [Range](../../../aspose.cells/range/)
* class [ExportRangeToJsonOptions](../../exportrangetojsonoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
## ExportRangeToJson(Range, JsonSaveOptions) {#exportrangetojson}
Exporting the range to json file.
```csharp
public static string ExportRangeToJson(Range range, JsonSaveOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | JsonSaveOptions | The options of exporting. |
### Return Value
The json string value.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class JsonUtilityMethodExportRangeToJsonWithRangeJsonSaveOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["C1"].PutValue("City");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["C2"].PutValue("New York");
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["C3"].PutValue("London");
// Create range (A1:C3)
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 3);
// Configure JSON export options
JsonSaveOptions options = new JsonSaveOptions();
options.ExportEmptyCells = true;
options.HasHeaderRow = true;
options.ExportNestedStructure = false;
// Export range to JSON
string jsonOutput = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options);
// Output the JSON result
Console.WriteLine(jsonOutput);
}
}
}
```
### See Also
* class [Range](../../../aspose.cells/range/)
* class [JsonSaveOptions](../../../aspose.cells/jsonsaveoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

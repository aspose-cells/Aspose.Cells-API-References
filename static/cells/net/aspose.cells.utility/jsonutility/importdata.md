##JsonUtility.ImportData
JsonUtility method. Import the json string
## JsonUtility.ImportData method
Import the json string.
```csharp
public static int[] ImportData(string json, Cells cells, int row, int column,
JsonLayoutOptions option)
```
| Parameter | Type | Description |
| --- | --- | --- |
| json | String | The json string. |
| cells | Cells | The Cells. |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| option | JsonLayoutOptions | The options of import json string. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonUtilityMethodImportDataWithStringCellsInt32Int32JsonLayouDemo
{
public static void Run()
{
string jsonInput = "[{"
+ "\"Name\" : \"Name\","
+ "\"DisplayName\" : \"DisplayName\","
+ "\"ShowDisplayName\" : false"
+ "},"
+ "{"
+ "\"Name\" : \"Nameone\","
+ "\"DisplayName\" : \"DisplayNameone\","
+ "\"ShowDisplayName\" : true"
+ "},"
+ "{"
+ "\"Name\" : \"Nametwo\","
+ "\"DisplayName\" : \"DisplayNametwo\","
+ "\"ShowDisplayName\" : false"
+ "}]";
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
JsonLayoutOptions options = new JsonLayoutOptions();
options.ArrayAsTable = true;
JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

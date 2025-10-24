##Class JsonLayoutOptions
Aspose.Cells.Utility.JsonLayoutOptions class. Represents the options of json layout type
## JsonLayoutOptions class
Represents the options of json layout type.
```csharp
public class JsonLayoutOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Constructor of loading JSON layout options. |
## Properties
| Name | Description |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Processes Array as table. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Indicates whether converting the string in json to numeric or date value. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Gets and sets the format of date value. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Indicates whether ignore title if array is a property of object. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Indicates whether ignoring null value. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Indicates whether ignore title if object is a property of object. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ingores titles of attributes |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Indicates whether keeping schema of this json. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Gets and sets the format of numeric value. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Gets and sets the style of the title. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class UtilityClassJsonLayoutOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create JsonLayoutOptions and set properties
JsonLayoutOptions options = new JsonLayoutOptions
{
ArrayAsTable = true,
ConvertNumericOrDate = true,
IgnoreArrayTitle = false,
IgnoreObjectTitle = false
};
// Sample JSON data
string jsonData = @"{
""Name"": ""John"",
""Age"": 30,
""Departments"": [""HR"", ""Finance"", ""IT""]
}";
// Import JSON data to worksheet
JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, options);
// Save the workbook
workbook.Save("JsonLayoutOptionsDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)

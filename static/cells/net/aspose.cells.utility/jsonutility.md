##Class JsonUtility
Aspose.Cells.Utility.JsonUtility class. Represents the utility class of processing json
## JsonUtility class
Represents the utility class of processing json.
```csharp
public class JsonUtility
```
## Constructors
| Name | Description |
| --- | --- |
| [JsonUtility](jsonutility/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson_1)(Range, ExportRangeToJsonOptions) | (**Obsolete.**) Exporting the range to json file. |
| static [ExportRangeToJson](../../aspose.cells.utility/jsonutility/exportrangetojson/#exportrangetojson)(Range, JsonSaveOptions) | Exporting the range to json file. |
| static [ImportData](../../aspose.cells.utility/jsonutility/importdata/)(string, Cells, int, int, JsonLayoutOptions) | Import the json string. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells.Utility;
using System;
public class JsonUtilityDemo
{
public static void JsonUtilityExample()
{
// Create an instance of JsonUtility
JsonUtility jsonUtility = new JsonUtility();
// Since the JsonUtility class does not have any properties or methods defined in the JSON,
// we will demonstrate its instantiation and potential usage contextually.
// Example: Assuming JsonUtility might be used for processing JSON data in some way.
// Note: The actual usage would depend on the methods and properties available in the real class.
// Here, we are just demonstrating the instantiation as no methods or properties are provided.
Console.WriteLine("JsonUtility instance created successfully.");
// Additional code to demonstrate potential usage
// For example, if JsonUtility had a method to process JSON, it might look like this:
// string jsonString = "{ \"name\": \"John\", \"age\": 30 }";
// var result = jsonUtility.ProcessJson(jsonString);
// Console.WriteLine("Processed JSON: " + result);
// Since no methods are provided, we will end the example here.
}
}
}
```
### See Also
* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)

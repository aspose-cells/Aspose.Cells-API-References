---
title: JsonLayoutOptions.JsonLayoutOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions constructor. Constructor of loading JSON layout options
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/jsonlayoutoptions/
---
## JsonLayoutOptions constructor

Constructor of loading JSON layout options.

```csharp
public JsonLayoutOptions()
```

### Examples

```csharp
// Called: JsonLayoutOptions options = new JsonLayoutOptions();
public void JsonLayoutOptions_Constructor()
{
    string path = Constants.TemplatePath + "NetCoreTests/CELLSNETCORE70/";
    string fileName = "JSON.txt";
    string json = "";
    using (System.IO.StreamReader file = System.IO.File.OpenText(path + fileName))
    {
        using (JsonTextReader reader = new JsonTextReader(file))
        {
            JObject o = (JObject)JToken.ReadFrom(reader);
            json = o.ToString();
        }
    }

    //Create workbook
    Workbook workbook = new Workbook();
    //Worksheet worksheet = workbook.Worksheets[0];

    //Read JSON files
    JsonLayoutOptions options = new JsonLayoutOptions();

    //Import JSON data
    JsonUtility.ImportData(json, workbook.Worksheets[0].Cells, 0, 0, options); //Error occurs here

    //Save Excel file
    DateTime today = DateTime.Now;
    workbook.Save(destPathNetCore + "example.xlsx");

}
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



---
title: JsonLayoutOptions.KeptSchema
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Indicates whether keeping schema of this json
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/keptschema/
---
## JsonLayoutOptions.KeptSchema property

Indicates whether keeping schema of this json.

```csharp
public bool KeptSchema { get; set; }
```

### Remarks

Sometimes we will save the file to JSON after loading JSON file.

### Examples

```csharp
// Called: layoutOptions.KeptSchema = true;
public void JsonLayoutOptions_Property_KeptSchema()
{
    var workbook = new Workbook();
    workbook.Worksheets.Clear();
    var worksheet = workbook.Worksheets.Add("1");

    var data1 = new Data()
    {
        RootProperty = "RootPropertyValue",
        Payload = new Payload()
        {
            Array = new[]
            {
        new ArrayData () { ArrayProperty = "a1" },
        new ArrayData () { ArrayProperty = "a2" },
        new ArrayData () { ArrayProperty = "a3" },
    },
            PayloadProperty = "PayloadPropertyValue",
            PayloadStruct = new PayloadStruct()
            {
                PayloadProperty1 = "val1",
                PayloadProperty2 = "val2"
            }
        }
    };

    var serializeObject = JsonConvert.SerializeObject(new[] { data1 });
    JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
    layoutOptions.KeptSchema = true;
    JsonUtility.ImportData(serializeObject, worksheet.Cells, 0, 0, layoutOptions);


    workbook.Save(Constants.destPath + "example.xlsx", SaveFormat.Xlsx);
    workbook.Save(Constants.destPath + "example.json", new JsonSaveOptions()
    {
        ExportNestedStructure = true,
        SkipEmptyRows = true,
        //   AlwaysExportAsJsonObject = true,
        ValidateMergedAreas = true,
    });
    string text = File.ReadAllText(Constants.destPath + "example.json");
    Assert.IsTrue(text.IndexOf("\"ArrayProperty\":\"a1\"") != -1);
}
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



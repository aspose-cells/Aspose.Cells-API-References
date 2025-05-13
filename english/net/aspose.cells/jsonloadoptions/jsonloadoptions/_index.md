---
title: JsonLoadOptions.JsonLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Creates an options of loading the file.

```csharp
public JsonLoadOptions()
```

### Examples

```csharp
// Called: JsonLoadOptions loadOptions = new JsonLoadOptions();
public void JsonLoadOptions_Constructor()
{
    JsonLoadOptions loadOptions = new JsonLoadOptions();
    loadOptions.KeptSchema = true;

    Workbook workbook = new Workbook(Constants.sourcePath + "example.json", loadOptions);

    workbook.Save(Constants.destPath + "example.xlsx");
      workbook = new Workbook(Constants.destPath + "example.xlsx");
    workbook.Save(Constants.destPath + "example.json", new JsonSaveOptions()
    {

        ExportNestedStructure = true,
        SkipEmptyRows = true,
          Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "example.json") }
        //  AlwaysExportAsJsonObject = true
    });
    Assert.IsTrue(File.ReadAllText(Constants.destPath + "example.json").IndexOf(" \"CurrencyConfigurations1\":[{") != -1);

}
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



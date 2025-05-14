---
title: JsonSaveOptions.JsonSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions constructor. Creates options for saving json file
type: docs
url: /net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Creates options for saving json file.

```csharp
public JsonSaveOptions()
```

### Examples

```csharp
// Called: JsonSaveOptions options = new JsonSaveOptions();
public void JsonSaveOptions_Constructor()
{
    Workbook w = new Workbook();


    JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
    //    layoutOptions.KeptSchema = true;
    JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + "example.json"), w.Worksheets[0].Cells, 0, 0, layoutOptions);


    JsonSaveOptions options = new JsonSaveOptions();
    options.Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "CellsNet56241_1_.schema") };
    options.ExportNestedStructure = true;
    options.SkipEmptyRows = true;
    //   AlwaysExportAsJsonObject = true,
    options.ValidateMergedAreas = true;

    w.Save(Constants.destPath + "example.json", options);
    string text = File.ReadAllText(Constants.destPath + "example.json");
    Assert.IsTrue(text.IndexOf("\"ArrayProperty\":\"a1\"") != -1);
}
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



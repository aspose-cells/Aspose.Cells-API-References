---
title: JsonSaveOptions.Schemas
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. The original json schema of each worksheet
type: docs
url: /net/aspose.cells/jsonsaveoptions/schemas/
---
## JsonSaveOptions.Schemas property

The original json schema of each worksheet.

```csharp
public string[] Schemas { get; set; }
```

### Examples

```csharp
// Called: options.Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "CellsNet56241_2.schema") };
public void JsonSaveOptions_Property_Schemas()
{
    Workbook w = new Workbook();


    JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
    //    layoutOptions.KeptSchema = true;
    JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + "example.json"), w.Worksheets[0].Cells, 0, 0, layoutOptions);


    JsonSaveOptions options = new JsonSaveOptions();
    options.Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "CellsNet56241_2.schema") };
    options.ExportNestedStructure = true;
    options.SkipEmptyRows = true;
    //   AlwaysExportAsJsonObject = true,
    options.ValidateMergedAreas = true;

    w.Save(Constants.destPath + "example.json", options);
    string text = File.ReadAllText(Constants.destPath + "example.json");
    Assert.IsTrue(text.IndexOf(" \"CurrencyConfigurations1\":[{") != -1);
}
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



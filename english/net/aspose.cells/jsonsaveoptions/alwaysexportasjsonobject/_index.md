---
title: JsonSaveOptions.AlwaysExportAsJsonObject
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether always exporting excel to json as object even there is only a worksheet in the file
type: docs
url: /net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Examples

```csharp
// Called: saveOptions.AlwaysExportAsJsonObject = true;
public void JsonSaveOptions_Property_AlwaysExportAsJsonObject()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    JsonSaveOptions saveOptions = new JsonSaveOptions();
    saveOptions.AlwaysExportAsJsonObject = true;
    saveOptions.ExportNestedStructure = true;
    saveOptions.SkipEmptyRows = true;
    workbook.Save(Constants.destPath + "example.json", saveOptions);
    string text = File.ReadAllText(Constants.destPath + "example.json");
    Assert.IsTrue(text.IndexOf("\"Sheet2\":[]") != -1);
}
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



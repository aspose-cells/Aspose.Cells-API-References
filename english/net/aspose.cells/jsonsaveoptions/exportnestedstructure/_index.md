---
title: JsonSaveOptions.ExportNestedStructure
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Exported as parentchild hierarchy Json structure
type: docs
url: /net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

Exported as parent-child hierarchy Json structure.

```csharp
public bool ExportNestedStructure { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportNestedStructure = true;
public void JsonSaveOptions_Property_ExportNestedStructure()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    JsonSaveOptions saveOptions = new JsonSaveOptions();
    saveOptions.AlwaysExportAsJsonObject = true;
    saveOptions.ExportNestedStructure = true;
    saveOptions.SkipEmptyRows = true;
    workbook.Save(Constants.destPath + "example.json", saveOptions);
    string text = File.ReadAllText(Constants.destPath + "example.json");
    Assert.IsTrue(text.IndexOf("null") == -1);
}
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



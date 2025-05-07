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
[Test]
        public void Property_ExportNestedStructure()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet52502.xlsx");
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            workbook.Save(Constants.destPath + "CellsNet52502.json", saveOptions);
            string text = File.ReadAllText(Constants.destPath + "CellsNet52502.json");
            Assert.IsTrue(text.StartsWith("{"));
            Assert.IsTrue(text.IndexOf("Sheet1") != -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



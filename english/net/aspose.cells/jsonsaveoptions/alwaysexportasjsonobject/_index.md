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
[Test]
        public void Property_AlwaysExportAsJsonObject()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet52502.xlsx&quot;);
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            workbook.Save(Constants.destPath + &quot;CellsNet52502.json&quot;, saveOptions);
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet52502.json&quot;);
            Assert.IsTrue(text.StartsWith(&quot;{&quot;));
            Assert.IsTrue(text.IndexOf(&quot;Sheet1&quot;) != -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



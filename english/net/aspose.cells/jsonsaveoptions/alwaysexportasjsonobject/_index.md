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
            Workbook book = new Workbook(Constants.sourcePath + "CELLSNET55579.xlsx");
            Aspose.Cells.Range range = book.Worksheets[0].Cells.CreateRange("A1:B2");

            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;
            string json = range.ToJson(saveOptions);
            Assert.IsTrue(json.IndexOf("\"cell\" :") > 0);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



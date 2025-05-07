---
title: JsonSaveOptions.ExportHyperlinkType
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Represents the type of exporting hyperlink to json
type: docs
url: /net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Represents the type of exporting hyperlink to json.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Remarks

The default value is DisplayString;

### Examples

```csharp
// Called: saveOptions.ExportHyperlinkType = Aspose.Cells.Json.JsonExportHyperlinkType.HtmlString;
[Test]
        public void Property_ExportHyperlinkType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET52344.htm");
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = Aspose.Cells.Json.JsonExportHyperlinkType.HtmlString;
            workbook.Save(Constants.destPath + "CELLSNET52344.json", saveOptions);
            string text = File.ReadAllText(Constants.destPath + "CELLSNET52344.json");
            Assert.IsTrue(text.IndexOf("www.intel.com") != -1);
        }
```

### See Also

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



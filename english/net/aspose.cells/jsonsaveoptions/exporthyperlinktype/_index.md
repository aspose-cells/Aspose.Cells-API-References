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
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET52344.htm&quot;);
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = Aspose.Cells.Json.JsonExportHyperlinkType.HtmlString;
            workbook.Save(Constants.destPath + &quot;CELLSNET52344.json&quot;, saveOptions);
            string text = File.ReadAllText(Constants.destPath + &quot;CELLSNET52344.json&quot;);
            Assert.IsTrue(text.IndexOf(&quot;www.intel.com&quot;) != -1);
        }
```

### See Also

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



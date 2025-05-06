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
            Workbook workbook = new Workbook(Constants.sourcePath + @&quot;json\CellsNet52242.json&quot;);
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            workbook.Save(Constants.destPath + &quot;CellsNet52242.json&quot;, saveOptions);

            workbook = new Workbook(Constants.destPath + &quot;CellsNet52242.json&quot;);
            Assert.AreEqual(&quot;&quot;, workbook.Worksheets[0].Cells[&quot;H10&quot;].StringValue);
            Assert.AreEqual(&quot;HighScenerio&quot;, workbook.Worksheets[0].Cells[&quot;J10&quot;].StringValue);
            Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



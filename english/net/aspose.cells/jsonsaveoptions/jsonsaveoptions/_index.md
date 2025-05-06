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
[Test]
        public void JsonSaveOptions_Constructor()
        {
            Workbook w = new Workbook();


            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            //    layoutOptions.KeptSchema = true;
            JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + &quot;CellsNet56241_2.json&quot;), w.Worksheets[0].Cells, 0, 0, layoutOptions);


            JsonSaveOptions options = new JsonSaveOptions();
            options.Schemas = new string[] { File.ReadAllText(Constants.sourcePath + &quot;CellsNet56241_2.schema&quot;) };
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            //   AlwaysExportAsJsonObject = true,
            options.ValidateMergedAreas = true;

            w.Save(Constants.destPath + &quot;CellsNet56241_2.json&quot;, options);
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet56241_2.json&quot;);
            Assert.IsTrue(text.IndexOf(&quot; \&quot;CurrencyConfigurations1\&quot;:[{&quot;) != -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: JsonSaveOptions.SkipEmptyRows
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether skipping emtpy rows
type: docs
url: /net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

Indicates whether skipping emtpy rows.

```csharp
public bool SkipEmptyRows { get; set; }
```

### Examples

```csharp
// Called: options.SkipEmptyRows = true;
[Test]
        public void Property_SkipEmptyRows()
        {
            Workbook w = new Workbook();


            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            //    layoutOptions.KeptSchema = true;
            JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + "CellsNet56241_1.json"), w.Worksheets[0].Cells, 0, 0, layoutOptions);


            JsonSaveOptions options = new JsonSaveOptions();
            options.Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "CellsNet56241_1_.schema") };
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            //   AlwaysExportAsJsonObject = true,
            options.ValidateMergedAreas = true;

            w.Save(Constants.destPath + "CellsNet56241_1.json", options);
            string text = File.ReadAllText(Constants.destPath + "CellsNet56241_1.json");
            Assert.IsTrue(text.IndexOf("\"ArrayProperty\":\"a1\"") != -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



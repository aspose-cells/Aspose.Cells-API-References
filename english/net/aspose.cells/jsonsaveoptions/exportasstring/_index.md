---
title: JsonSaveOptions.ExportAsString
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Exports the string value of the cells to json
type: docs
url: /net/aspose.cells/jsonsaveoptions/exportasstring/
---
## JsonSaveOptions.ExportAsString property

Exports the string value of the cells to json.

```csharp
public bool ExportAsString { get; set; }
```

### Examples

```csharp
// Called: exportOptions.ExportAsString = true;
[Test]
        public void Property_ExportAsString()
        {
            Workbook wb = new Workbook();
            string str = File.ReadAllText(Constants.sourcePath + &quot;CellsNet47113.json&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            JsonLayoutOptions importOptions = new JsonLayoutOptions();
            importOptions.ConvertNumericOrDate = true;
            importOptions.ArrayAsTable = true;
            JsonUtility.ImportData(str, cells, 0, 0, importOptions);
            wb.Save(Constants.destPath + &quot;CellsNet47113.csv&quot;);
            Aspose.Cells.Range range = cells.MaxDisplayRange;
            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;
            
            string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace(&quot;\r\n&quot;, &quot;\n&quot;), ext.Replace(&quot;\r\n&quot;, &quot;\n&quot;));
            TxtLoadOptions textLoadOptions = new TxtLoadOptions();
            textLoadOptions.Separator = &apos;,&apos;;


            wb = new Workbook(Constants.sourcePath + &quot;CellsNet47113.csv&quot;, textLoadOptions);
            cells = wb.Worksheets[0].Cells;
            range = cells.MaxDisplayRange;
            exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace(&quot;\r\n&quot;, &quot;\n&quot;), ext.Replace(&quot;\r\n&quot;, &quot;\n&quot;));
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



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
            string str = File.ReadAllText(Constants.sourcePath + "CellsNet47113.json");
            Cells cells = wb.Worksheets[0].Cells;
            JsonLayoutOptions importOptions = new JsonLayoutOptions();
            importOptions.ConvertNumericOrDate = true;
            importOptions.ArrayAsTable = true;
            JsonUtility.ImportData(str, cells, 0, 0, importOptions);
            wb.Save(Constants.destPath + "CellsNet47113.csv");
            Aspose.Cells.Range range = cells.MaxDisplayRange;
            JsonSaveOptions exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;
            
            string ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace("\r\n", "\n"), ext.Replace("\r\n", "\n"));
            TxtLoadOptions textLoadOptions = new TxtLoadOptions();
            textLoadOptions.Separator = ',';


            wb = new Workbook(Constants.sourcePath + "CellsNet47113.csv", textLoadOptions);
            cells = wb.Worksheets[0].Cells;
            range = cells.MaxDisplayRange;
            exportOptions = new JsonSaveOptions();
            exportOptions.ExportAsString = true;

            ext = JsonUtility.ExportRangeToJson(range, exportOptions);
            Assert.AreEqual(str.Replace("\r\n", "\n"), ext.Replace("\r\n", "\n"));
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



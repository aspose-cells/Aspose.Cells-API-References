---
title: JsonLayoutOptions.ArrayAsTable
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Processes Array as table
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Processes Array as table.

```csharp
public bool ArrayAsTable { get; set; }
```

### Examples

```csharp
// Called: options.ArrayAsTable = true;
[Test]
        public void Property_ArrayAsTable()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreTitle = true;// **
            string jsonData = File.ReadAllText(Constants.sourcePath + &quot;CellsNet52281.json&quot;);
            JsonUtility.ImportData(jsonData, sheet.Cells, 0, 0, options);
            Assert.AreEqual(2,workbook.Worksheets[0].Cells.Rows.Count);
            workbook.Save(Constants.destPath + &quot;CellsNet52281.xlsx&quot;);
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



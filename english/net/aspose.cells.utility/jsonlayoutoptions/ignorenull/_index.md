---
title: JsonLayoutOptions.IgnoreNull
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Indicates whether ignoring null value
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/ignorenull/
---
## JsonLayoutOptions.IgnoreNull property

Indicates whether ignoring null value.

```csharp
public bool IgnoreNull { get; set; }
```

### Examples

```csharp
// Called: options.IgnoreNull = true;
public void Property_IgnoreNull()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            string json = File.ReadAllText(Constants.sourcePath + "CELLSNET46553.bd5");
             JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.IgnoreNull = true;

            options.IgnoreTitle = true;
            options.NumberFormat = "$0.00";
            options.ConvertNumericOrDate = true;
            JsonUtility.ImportData(json, cells, 0, 0, options);
            Assert.AreEqual(cells["E2"].StringValue, "$500.00");
            Assert.AreEqual("sun1.opacity = (sun1.opacity / 100) * 90;", cells["R2"].StringValue);
            Assert.AreEqual("$36.00", cells["L2"].StringValue);
            workbook.Save(Constants.destPath + "CELLSNET46553.xlsx");
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



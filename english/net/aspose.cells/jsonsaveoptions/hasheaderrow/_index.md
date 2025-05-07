---
title: JsonSaveOptions.HasHeaderRow
second_title: Aspose.Cells for .NET API Reference
description: JsonSaveOptions property. Indicates whether the range contains header row
type: docs
url: /net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Indicates whether the range contains header row.

```csharp
public bool HasHeaderRow { get; set; }
```

### Examples

```csharp
// Called: ops.HasHeaderRow = true;
[Test]
        public void Property_HasHeaderRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +"CellsNet52498.xlsx");
            var ops = new Aspose.Cells.JsonSaveOptions();
            ops.ExportNestedStructure = true; // if remove this line or fill a string like 'ID' into first cell, it's OK.
            ops.HasHeaderRow = true;
            workbook.Save(Constants.destPath + "CellsNet52498.json", ops);
            string text = File.ReadAllText(Constants.destPath + "CellsNet52498.json");
            Assert.IsTrue(text.IndexOf("\"1\"") != -1);
        }
```

### See Also

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



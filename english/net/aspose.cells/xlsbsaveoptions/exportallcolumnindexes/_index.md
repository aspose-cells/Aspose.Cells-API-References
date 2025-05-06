---
title: XlsbSaveOptions.ExportAllColumnIndexes
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions property. Indicates whether exporting all column indexes for cells
type: docs
url: /net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Indicates whether exporting all column indexes for cells.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
// Called: saveOptions.ExportAllColumnIndexes = false;
[Test]
        public void Property_ExportAllColumnIndexes()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;A1&quot;);
            cells[&quot;B1&quot;].PutValue(&quot;B1&quot;);
            cells[&quot;C1&quot;].PutValue(&quot;C1&quot;);
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;
            workbook.Save(Constants.destPath + &quot;ExportColumnIndexes001.xlsb&quot;, saveOptions);
            saveOptions.ExportAllColumnIndexes = false;
            workbook.Save(Constants.destPath + &quot;ExportColumnIndexes002.xlsb&quot;, saveOptions);
        }
```

### See Also

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



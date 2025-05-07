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
// Called: saveOptions.ExportAllColumnIndexes = true;
[Test]
        public void Property_ExportAllColumnIndexes()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("A1");
            cells["B1"].PutValue("B1");
            cells["C1"].PutValue("C1");
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;
            workbook.Save(Constants.destPath + "ExportColumnIndexes001.xlsb", saveOptions);
            saveOptions.ExportAllColumnIndexes = false;
            workbook.Save(Constants.destPath + "ExportColumnIndexes002.xlsb", saveOptions);
        }
```

### See Also

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



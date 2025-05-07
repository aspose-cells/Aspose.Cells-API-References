---
title: ExportTableOptions.FormatStrategy
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Gets and sets the format strategy when exporting the value as string value
type: docs
url: /net/aspose.cells/exporttableoptions/formatstrategy/
---
## ExportTableOptions.FormatStrategy property

Gets and sets the format strategy when exporting the value as string value.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Examples

```csharp
// Called: etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
[Test]
        public void Property_FormatStrategy()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23");
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23356");
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), "1.23");
        }
```

### See Also

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



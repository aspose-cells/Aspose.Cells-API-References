---
title: ExportTableOptions.ExportAsString
second_title: Aspose.Cells for .NET API Reference
description: ExportTableOptions property. Exports the string value of the cells to the DataTable
type: docs
url: /net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Exports the string value of the cells to the DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Examples

```csharp
// Called: etOpt.ExportAsString = true;
[Test]
        public void Property_ExportAsString()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(1.23356);
            Style style = cells[&quot;A1&quot;].GetStyle();
            style.Custom = &quot;0.00&quot;;
            cells[&quot;A1&quot;].SetStyle(style);
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), &quot;1.23&quot;);
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), &quot;1.23356&quot;);
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Assert.AreEqual(dt.Rows[0][0].ToString(), &quot;1.23&quot;);
        }
```

### See Also

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



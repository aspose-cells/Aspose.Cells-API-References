---
title: HtmlSaveOptions.ExportHiddenWorksheet
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating if exporting the hidden worksheet content.The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indicating if exporting the hidden worksheet content.The default value is true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Examples

```csharp
// Called: ExportHiddenWorksheet = false,
[Test]
        public void Property_ExportHiddenWorksheet()
        {
            Workbook workbook = new Workbook(Constants.HtmlPath + &quot;CELLSNET-50997.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            sheet.PageSetup.PrintArea = &quot;D5:L65&quot;;

            var htmlSaveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false,
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportWorkbookProperties = false,
            };

            sheet.Workbook.Save(_destFilesPath + &quot;CELLSNET-50997_Cs.html&quot;, htmlSaveOptions);

            Workbook reloadWorkbook = new Workbook(_destFilesPath + &quot;CELLSNET-50997_Cs.html&quot;);

            Cells cells = reloadWorkbook.Worksheets[0].Cells;
            Style I8Style = cells[&quot;I8&quot;].GetStyle(true);
            Assert.AreEqual(CellBorderType.Dotted, I8Style.Borders[BorderType.LeftBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, I8Style.Borders[BorderType.RightBorder].LineStyle);

            Style I38Style = cells[&quot;I38&quot;].GetStyle(true);
            Assert.AreEqual(CellBorderType.Dotted, I38Style.Borders[BorderType.LeftBorder].LineStyle);
            Assert.AreEqual(CellBorderType.None, I38Style.Borders[BorderType.RightBorder].LineStyle);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



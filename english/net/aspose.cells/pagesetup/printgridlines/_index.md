---
title: PageSetup.PrintGridlines
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents if cell gridlines are printed on the page
type: docs
url: /net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Represents if cell gridlines are printed on the page.

```csharp
public bool PrintGridlines { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.PrintGridlines = false;
[Test]
        public void Property_PrintGridlines()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET50778_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;VERKAUF_Pivot_Excel2010.xls&quot;);

            foreach (Worksheet worksheet in wb.Worksheets)
            {
                worksheet.PageSetup.PrintGridlines = false;
            }

            // create explicit SaveOptions
            Aspose.Cells.PdfSaveOptions pdfSaveOptions = new Aspose.Cells.PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.ExportDocumentStructure = true;

            //wb.Worksheets.RefreshPivotTables();
            wb.Save(savePath + &quot;out.pdf&quot;, pdfSaveOptions);

            Style b11Style = wb.Worksheets[1].Cells[&quot;B11&quot;].GetStyle();
            Assert.AreEqual(b11Style.Borders[BorderType.LeftBorder].LineStyle, CellBorderType.Thin);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



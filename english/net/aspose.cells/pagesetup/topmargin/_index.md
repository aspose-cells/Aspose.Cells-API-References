---
title: PageSetup.TopMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the top margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Represents the size of the top margin, in unit of centimeters.

```csharp
public double TopMargin { get; set; }
```

### Examples

```csharp
// Called: wks.PageSetup.TopMargin = 1;
[Test]
        public void Property_TopMargin()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            htmlLoadOptions.AutoFitColsAndRows = true;

            Workbook workbook = new Workbook(Constants.HtmlPath + "CELLSNET-50328.xls", htmlLoadOptions);
            Aspose.Cells.PdfSaveOptions pdfSaveOptions = new Aspose.Cells.PdfSaveOptions();
            // option to set all the columns of excel in one page.
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.MergeAreas = true;
            /* Retain the structure of original excel */
            pdfSaveOptions.ExportDocumentStructure = true;
            /* Formula calculation for any digit formulla applied in excels */
            /*it is best to call Workbook.CalculateFormula() just before rendering the spreadsheet to PDF. 
           * This ensures  that the formula dependent values are recalculated, and the correct
           * values are rendered in the PDF.*/
            workbook.CalculateFormula();


            foreach (Worksheet wks in workbook.Worksheets)
            {
                wks.PageSetup.PrintArea = "";
                wks.PageSetup.BottomMargin = 1;
                wks.PageSetup.LeftMargin = 1;
                wks.PageSetup.RightMargin = 1;
                wks.PageSetup.TopMargin = 1;
            }

            int maxDataRow = workbook.Worksheets[0].Cells.MaxDataRow;
            Cell cell = workbook.Worksheets[0].Cells[maxDataRow - 2, 0];
            Assert.AreEqual(0, cell.GetStyle().ForegroundArgbColor);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



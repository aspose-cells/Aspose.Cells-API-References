---
title: PdfSaveOptions.PdfCompression
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Indicate the compression algorithm
type: docs
url: /net/aspose.cells/pdfsaveoptions/pdfcompression/
---
## PdfSaveOptions.PdfCompression property

Indicate the compression algorithm

```csharp
public PdfCompressionCore PdfCompression { get; set; }
```

### Examples

```csharp
// Called: saveOptions.PdfCompression = PdfCompressionCore.Flate;
[Test]
        public void Property_PdfCompression()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43846_";
            Workbook wb = new Workbook(filePath + "Source File.xlsx");
            //If you dont refresh this pivot table, excel file does not get corrupted, else it does.
            Worksheet targetSheet = wb.Worksheets["PivotTable"];
            PivotTable _pivotTable = targetSheet.PivotTables[0];
            PivotField field = _pivotTable.PageFields["Producer"];
            for (int i = 0; i <= field.PivotItems.Count - 1; i++)
            {
                if (field.PivotItems[i].GetStringValue().Equals("ABC"))
                {
                    field.CurrentPageItem = (short)i;
                }
            }

            _pivotTable.RefreshData();
            _pivotTable.CalculateData();

            Cells cells = targetSheet.Cells;
            Assert.AreEqual(cells["D7"].StringValue, "0");
            Assert.AreEqual(cells["D8"].StringValue, "0");
            Assert.AreEqual(cells["D9"].StringValue, "0");
            Assert.AreEqual(cells["F7"].StringValue, "137.7755");
            Assert.AreEqual(cells["F8"].StringValue, "434.784");
            Assert.AreEqual(cells["F9"].StringValue, "572.5595");

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.AllColumnsInOnePagePerSheet = true;
            saveOptions.PdfCompression = PdfCompressionCore.Flate;
            saveOptions.RefreshChartCache = true;

            wb.Save(CreateFolder(filePath) + "out.pdf", saveOptions);
            wb.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* enum [PdfCompressionCore](../../../aspose.cells.rendering/pdfcompressioncore/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



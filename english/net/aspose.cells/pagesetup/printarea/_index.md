---
title: PageSetup.PrintArea
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the range to be printed
type: docs
url: /net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Represents the range to be printed.

```csharp
public string PrintArea { get; set; }
```

### Examples

```csharp
// Called: workbook.Worksheets[index].PageSetup.PrintArea = range;
private void PageSetup_Property_PrintArea(int index,string range)
        {

            Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xlsx");
            var htmlSaveOptions = new HtmlSaveOptions
            {
                Encoding = Encoding.UTF8,
                ExportImagesAsBase64 = true,
                ExportPrintAreaOnly = true,
                ExportActiveWorksheetOnly = true,
                ExportWorksheetCSSSeparately = false,
                ExcludeUnusedStyles = true,
                ExportDocumentProperties = false,
                ExportWorkbookProperties = false,
                ExportSimilarBorderStyle = true,
            };
            workbook.Worksheets.ActiveSheetIndex = index;
            workbook.Worksheets[index].PageSetup.PrintArea = range;

            workbook.Save(Constants.destPath + "CELLSNETCORE269_"+index+".html", htmlSaveOptions);
            workbook = new Workbook(Constants.destPath + "CELLSNETCORE269_" + index + ".html");
            Assert.AreEqual(2, workbook.Worksheets[0].Cells["B2"].IntValue);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



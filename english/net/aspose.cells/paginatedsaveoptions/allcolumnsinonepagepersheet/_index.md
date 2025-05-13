---
title: PaginatedSaveOptions.AllColumnsInOnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. If AllColumnsInOnePagePerSheet is true  all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
public void PaginatedSaveOptions_Property_AllColumnsInOnePagePerSheet()
{
    string filePath = Constants.PivotTableSourcePath + @"NET50778_";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "example.xls");

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
    wb.Save(savePath + "out.pdf", pdfSaveOptions);

    Style b11Style = wb.Worksheets[1].Cells["B11"].GetStyle();
    Assert.AreEqual(b11Style.Borders[BorderType.LeftBorder].LineStyle, CellBorderType.Thin);
}
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



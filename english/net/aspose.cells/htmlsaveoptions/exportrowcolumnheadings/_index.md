---
title: HtmlSaveOptions.ExportRowColumnHeadings
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exports sheets row and column headings when saving to HTML files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportrowcolumnheadings/
---
## HtmlSaveOptions.ExportRowColumnHeadings property

Indicates whether exports sheet's row and column headings when saving to HTML files.

```csharp
public bool ExportRowColumnHeadings { get; set; }
```

### Remarks

The default value is false.

### Examples

```csharp
// Called: saveOptions.ExportRowColumnHeadings = false;
public void HtmlSaveOptions_Property_ExportRowColumnHeadings()
{
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportPrintAreaOnly = true;
    saveOptions.ExportActiveWorksheetOnly = true;
    saveOptions.ExportImagesAsBase64 = true;
    saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
    saveOptions.DefaultFontName = null;
    saveOptions.IsExportComments = false;
    saveOptions.ExportRowColumnHeadings = false;
    saveOptions.ExportExtraHeadings = true;
    saveOptions.ExportGridLines = false;
    saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
    saveOptions.CellCssPrefix = "p1-65dd5c19f29-";

    Workbook wb = new Workbook(Constants.HtmlPath + "example.xlsx");
    WorksheetCollection sheets = wb.Worksheets;
    string destPath = _destFilesPath + "CELLSNET-56578";
    if (!Directory.Exists(destPath))
        Directory.CreateDirectory(destPath);
    for (int i = 0; i < sheets.Count; i++)// sheets.Count is growing in trial mode
    {
        Worksheet one = sheets[i];
        saveOptions.TableCssId = "gdt-id-" + (i + 1).ToString();
        one.IsSelected = true;
        wb.Worksheets.ActiveSheetIndex = one.Index;
        Console.WriteLine("Saving worksheet {0} - '{1}'", one.Index, one.Name);
        string outputFilename = destPath + string.Format("example.html", one.Index, one.Name);
        wb.Save(outputFilename, saveOptions); // exception here
    }
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



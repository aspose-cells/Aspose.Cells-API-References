---
title: HtmlSaveOptions.TableCssId
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets and sets the prefix of the type css name such as trcoltd and so on they are contained in the table element which has the specific TableCssId attribute. The default value is 
type: docs
url: /net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".

```csharp
public string TableCssId { get; set; }
```

### Examples

```csharp
// Called: saveOptions.TableCssId = "gdt-id-" + (i + 1).ToString();
[Test]
        public void Property_TableCssId()
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

            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-56578.xlsx");
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
                string outputFilename = destPath + string.Format("CELLSNET-56578_{0}_{1}.html", one.Index, one.Name);
                wb.Save(outputFilename, saveOptions); // exception here
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



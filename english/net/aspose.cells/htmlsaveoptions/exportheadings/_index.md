---
title: HtmlSaveOptions.ExportHeadings
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exports sheets row and column headings when saving to HTML files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Indicates whether exports sheet's row and column headings when saving to HTML files.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use HtmlSaveOptions.ExportRowColumnHeadings property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: options.ExportHeadings = true;
[Test]
        public void Property_ExportHeadings()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET48131/";
            Workbook wb = new Workbook(filePath + "Sample Check Register.xlsx");
            Worksheet ws = wb.Worksheets[0];

            wb.Worksheets.ActiveSheetIndex = 0;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHiddenWorksheet = false;
            options.ExportActiveWorksheetOnly = true;
            options.HtmlCrossStringType = HtmlCrossType.Cross;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.CellCssPrefix = "prefix";
            options.ExportImagesAsBase64 = true;

            options.ExportHeadings = true;
            options.ExportExtraHeadings = true;
            options.ExportGridLines = true;

            wb.Save(_destFilesPath + "NET48131.html", options);
            string text = File.ReadAllText(_destFilesPath + "NET48131.html");
            Assert.IsTrue(text.IndexOf("z-index:2;margin-left:11px;margin-top:26px;width:379px;height:320px'") != -1);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



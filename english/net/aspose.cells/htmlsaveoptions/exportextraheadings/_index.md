---
title: HtmlSaveOptions.ExportExtraHeadings
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Examples

```csharp
// Called: options.ExportExtraHeadings = true;
[Test]
        public void Property_ExportExtraHeadings()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET48085/";
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + "Hidden table header.xlsx");
            wb.Worksheets.ActiveSheetIndex = 0;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.IsExpImageToTempDir = true;
            options.ExportHeadings = true;
            options.ExportExtraHeadings = true;
            options.ExportGridLines = true;

            wb.Save(savePath + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



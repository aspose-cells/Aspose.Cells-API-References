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
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET48131/&quot;;
            Workbook wb = new Workbook(filePath + &quot;Sample Check Register.xlsx&quot;);
            Worksheet ws = wb.Worksheets[0];

            wb.Worksheets.ActiveSheetIndex = 0;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHiddenWorksheet = false;
            options.ExportActiveWorksheetOnly = true;
            options.HtmlCrossStringType = HtmlCrossType.Cross;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.CellCssPrefix = &quot;prefix&quot;;
            options.ExportImagesAsBase64 = true;

            options.ExportHeadings = true;
            options.ExportExtraHeadings = true;
            options.ExportGridLines = true;

            wb.Save(_destFilesPath + &quot;NET48131.html&quot;, options);
            string text = File.ReadAllText(_destFilesPath + &quot;NET48131.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;z-index:2;margin-left:11px;margin-top:26px;width:379px;height:320px&apos;&quot;) != -1);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



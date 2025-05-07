---
title: HtmlSaveOptions.IsExpImageToTempDir
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting image files to temp directory. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Examples

```csharp
// Called: options.IsExpImageToTempDir = true;
[Test]
        public void Property_IsExpImageToTempDir()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45621/";

            Workbook wb = new Workbook(filePath + "Input.xls");

            wb.Worksheets.ActiveSheetIndex = 0;

            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            options.ExportDataOptions = HtmlExportDataOptions.All;
            options.IsExpImageToTempDir = true;
            wb.Save(CreateFolder(filePath) + "out.html");
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



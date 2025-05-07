---
title: HtmlSaveOptions.ExportGridLines
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting the gridlines.The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Indicating whether exporting the gridlines.The default value is false.

```csharp
public bool ExportGridLines { get; set; }
```

### Examples

```csharp
// Called: ExportGridLines = true
[Test]
        public void Property_ExportGridLines()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47609/";
            string savePath = CreateFolder(filePath);

            var options = new HtmlSaveOptions
            {
                ExportImagesAsBase64 = true,
                ExportSingleTab = true,
                ExportGridLines = true
            };

            Workbook wb = null;
            wb = new Workbook(filePath + "withOtherContent.xlsx");
            wb.Save(savePath + "out.html", options);

            wb = new Workbook(filePath + "noOtherContent.xlsx");
            wb.Save(savePath + "out2.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: HtmlSaveOptions.ImageScalable
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/imagescalable/
---
## HtmlSaveOptions.ImageScalable property

Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.

```csharp
public bool ImageScalable { get; set; }
```

### Examples

```csharp
// Called: opts.ImageScalable = false;
[Test]
        public void Property_ImageScalable()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43272/";
            string savePath = CreateFolder(filePath);

            HtmlSaveOptions opts = new HtmlSaveOptions();
            opts.WidthScalable = true;
            opts.ImageScalable = false;
            opts.ExportActiveWorksheetOnly = true;
            opts.ExportImagesAsBase64 = true;

            Workbook wb = new Workbook(filePath + "TL_Summary_Report_Template.xlsx");
            wb.Save(savePath + "out.html", opts);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



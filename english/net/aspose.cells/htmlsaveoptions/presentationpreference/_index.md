---
title: HtmlSaveOptions.PresentationPreference
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentationplease set the value to true
type: docs
url: /net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.

```csharp
public bool PresentationPreference { get; set; }
```

### Examples

```csharp
// Called: options.PresentationPreference = true;
[Test]
        public void Property_PresentationPreference()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43076/";

            Workbook wb = new Workbook(filePath + "DataAndChart.xlsx");

            wb.Worksheets.ActiveSheetIndex = 0;
            // export the worksheet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            options.Encoding = Encoding.UTF8;
            options.PresentationPreference = true;
            options.ExportActiveWorksheetOnly = true;
            options.ExportImagesAsBase64 = true;


            // *tries* to set the Chart Shape to SVG@ 300DPI, but results in PNG
            ImageOrPrintOptions imgOptions = options.ImageOptions;
            imgOptions.ImageType = ImageType.Svg;
            imgOptions.HorizontalResolution = 300;
            imgOptions.VerticalResolution = 300;

            wb.Save(CreateFolder(filePath) + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



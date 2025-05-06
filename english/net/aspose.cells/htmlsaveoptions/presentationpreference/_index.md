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
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43578/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook workbook = new Workbook(filePath + &quot;excel转换后部分格式变形错误.xlsx&quot;);

            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            //Add this line to ignore hidden columns when automatically adjusting column widths
            autoFitterOptions.IgnoreHidden = true;

            WorksheetCollection sheetCollection = workbook.Worksheets;
            int sheetCont = sheetCollection.Count;
            for (int i = 0; i &lt; sheetCont; i++)
            {
                sheetCollection[i].AutoFitColumns(autoFitterOptions);
            }

            HtmlSaveOptions options = new HtmlSaveOptions();

            options.ExportDocumentProperties = false;
            options.ExportWorkbookProperties = false;
            options.ExportWorksheetProperties = false;
            options.ExportSimilarBorderStyle = true;
            options.ExportImagesAsBase64 = false;
            options.ExcludeUnusedStyles = true;
            options.ExportHiddenWorksheet = false;
            options.WidthScalable = false;
            options.PresentationPreference = true;

            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
            workbook.Save(savePath + &quot;out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



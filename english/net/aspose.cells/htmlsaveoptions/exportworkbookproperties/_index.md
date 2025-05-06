---
title: HtmlSaveOptions.ExportWorkbookProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportWorkbookProperties = false;
[Test]
        public void Property_ExportWorkbookProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43558/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook workbook = new Workbook(filePath + &quot;excel转换后隐藏列被显示.xlsx&quot;);

            WorksheetCollection sheetCollection = workbook.Worksheets;
            int sheetCont = sheetCollection.Count;
            AutoFitterOptions autoFitOptions = new AutoFitterOptions();
            autoFitOptions.IgnoreHidden = true;
            for (int i = 0; i &lt; sheetCont; i++)
            {
                sheetCollection[i].AutoFitColumns(autoFitOptions);
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
            //Following options also do not work
            options.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            workbook.Save(savePath + &quot;out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



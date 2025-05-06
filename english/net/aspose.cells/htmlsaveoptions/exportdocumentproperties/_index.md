---
title: HtmlSaveOptions.ExportDocumentProperties
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Examples

```csharp
// Called: options.ExportDocumentProperties = false;
[Test]
        public void Property_ExportDocumentProperties()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43397/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;2020年1月第2周计划.xlsx&quot;);
            WorksheetCollection sheetCollection = wb.Worksheets;
            int sheetCont = sheetCollection.Count;
            for (int i = 0; i &lt; sheetCont; i++)
            {
                sheetCollection[i].AutoFitColumns();
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
            wb.Save(savePath + &quot;out.xlsx&quot;);
            wb.Save(savePath + &quot;out.html&quot;, options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



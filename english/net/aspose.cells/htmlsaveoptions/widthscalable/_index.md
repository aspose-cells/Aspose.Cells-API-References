---
title: HtmlSaveOptions.WidthScalable
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting column width in unit of scale to html. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Indicates whether exporting column width in unit of scale to html. The default value is false.

```csharp
public bool WidthScalable { get; set; }
```

### Examples

```csharp
// Called: options.WidthScalable = false;
[Test]
        public void Property_WidthScalable()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43397/";
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + "2020年1月第2周计划.xlsx");
            WorksheetCollection sheetCollection = wb.Worksheets;
            int sheetCont = sheetCollection.Count;
            for (int i = 0; i < sheetCont; i++)
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
            wb.Save(savePath + "out.xlsx");
            wb.Save(savePath + "out.html", options);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



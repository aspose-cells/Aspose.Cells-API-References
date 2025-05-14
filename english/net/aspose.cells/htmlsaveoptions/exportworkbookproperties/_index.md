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
public void HtmlSaveOptions_Property_ExportWorkbookProperties()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA43397/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "example.xlsx");
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



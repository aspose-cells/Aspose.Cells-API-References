---
title: HtmlSaveOptions.ExportWorksheetCSSSeparately
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether export the worksheet css separately.The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Indicating whether export the worksheet css separately.The default value is false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportWorksheetCSSSeparately = true;
public void HtmlSaveOptions_Property_ExportWorksheetCSSSeparately()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47092/";

    string savePath = CreateFolder(filePath);
    Workbook wb = new Workbook(filePath + "SampleFile.xlsx");

    Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
    htmlSaveOptions.ExportWorksheetCSSSeparately = true;
    htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
    htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
    htmlSaveOptions.StreamProvider = new ExportStreamProvider(savePath);
    htmlSaveOptions.DisableDownlevelRevealedComments = true;
    htmlSaveOptions.ExportImagesAsBase64 = false;//it is not working anyway!!!

    htmlSaveOptions.ExportActiveWorksheetOnly = true;
    wb.Worksheets.ActiveSheetIndex = 0;


    wb.Save(savePath + "out.html", htmlSaveOptions);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



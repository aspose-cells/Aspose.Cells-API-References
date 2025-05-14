---
title: HtmlSaveOptions.ExportActiveWorksheetOnly
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file If false then the whole workbook will be exported to html file. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indicates if only exporting the active worksheet to html file. If true then only the active worksheet will be exported to html file; If false then the whole workbook will be exported to html file. The default value is false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportActiveWorksheetOnly = true;
public void HtmlSaveOptions_Property_ExportActiveWorksheetOnly()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47578/";
    string savePath = CreateFolder(filePath);

    Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
    htmlSaveOptions.ExportWorksheetCSSSeparately = true;
    htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
    htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
    htmlSaveOptions.DisableDownlevelRevealedComments = true;
    htmlSaveOptions.ExportImagesAsBase64 = false;
    htmlSaveOptions.ExportActiveWorksheetOnly = true;

    Aspose.Cells.LoadOptions loadOptions = new Aspose.Cells.LoadOptions(Aspose.Cells.LoadFormat.Auto);

    using (Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(filePath + "test.xlsb", loadOptions))
    {
        workbook.Worksheets.ActiveSheetIndex = 0;

        workbook.Save(savePath + "out.html", htmlSaveOptions);
    }
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



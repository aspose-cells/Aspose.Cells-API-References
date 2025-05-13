---
title: HtmlSaveOptions.ExportDataOptions
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating the rule of exporting html file data.The default value is All
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Indicating the rule of exporting html file data.The default value is All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
public void HtmlSaveOptions_Property_ExportDataOptions()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET44088/";

    string savePath = CreateFolder(filePath);
    Aspose.Cells.Workbook wb = new Workbook(filePath + "SampleFile.xlsx");
    wb.Save(savePath + "out.pdf");

    Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
    htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
    htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
    wb.Save(savePath + "out.html", htmlSaveOptions);

    wb = new Workbook(filePath + "a2.xlsx");
    wb.Save(savePath + "a2_out.html", htmlSaveOptions);
    wb.Save(savePath + "a2_out.pdf");

    wb = new Workbook(filePath + "a3.xlsx");
    wb.Save(savePath + "a3_out.html", htmlSaveOptions);
    wb.Save(savePath + "a3_out.pdf");
}
```

### See Also

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: HtmlSaveOptions.ExportExtraHeadings
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportextraheadings/
---
## HtmlSaveOptions.ExportExtraHeadings property

Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.

```csharp
public bool ExportExtraHeadings { get; set; }
```

### Examples

```csharp
// Called: options.ExportExtraHeadings = true;
public void HtmlSaveOptions_Property_ExportExtraHeadings()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET47674/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "sample.xlsx");
    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportDataOptions = HtmlExportDataOptions.All;
    options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;
    options.ExportHeadings = true;
    options.ExportExtraHeadings = true;
    wb.Save(savePath + "out.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



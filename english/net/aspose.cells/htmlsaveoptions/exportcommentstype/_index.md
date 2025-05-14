---
title: HtmlSaveOptions.ExportCommentsType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Represents type of exporting comments to html files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Represents type of exporting comments to html files.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
public void HtmlSaveOptions_Property_ExportCommentsType()
{
    Workbook workbook = new Workbook(Constants.HtmlSourcePath + "example.xlsx");
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
    workbook.Save(Constants.HtmlDestPath + "example.html", saveOptions);
    string text = File.ReadAllText(Constants.HtmlDestPath + "example.html");
    Assert.IsTrue(text.IndexOf("<br/>who am i<br/>") != -1);
}
```

### See Also

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



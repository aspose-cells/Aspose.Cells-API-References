---
title: HtmlSaveOptions.ExportHiddenWorksheet
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating if exporting the hidden worksheet content.The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indicating if exporting the hidden worksheet content.The default value is true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Examples

```csharp
// Called: ExportHiddenWorksheet = false,
public void HtmlSaveOptions_Property_ExportHiddenWorksheet()
{


    var workbook = new Workbook(Constants.sourcePath + @"example.xlsx");
    var htmlSaveOptions = new HtmlSaveOptions
    {
        ExportHiddenWorksheet = false,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
        ExportActiveWorksheetOnly = true
    };
    workbook.Save(Constants.destPath + @"example.html", htmlSaveOptions);
    workbook = new Workbook(Constants.destPath + @"example.html");
    Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Korea");
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: HtmlLoadOptions.AutoFitColsAndRows
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether autofit columns and rows. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indicates whether auto-fit columns and rows. The default value is false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Examples

```csharp
// Called: loadOptions.AutoFitColsAndRows = true;
public void HtmlLoadOptions_Property_AutoFitColsAndRows()
{
    HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
    Workbook wb = new Workbook(Constants.HtmlPath + "example.html", loadOptions);
    loadOptions.AutoFitColsAndRows = true;
    loadOptions.ConvertNumericData = false;
    Style style = wb.Worksheets[0].Cells["A13"].GetStyle();
    Assert.AreEqual(style.HorizontalAlignment, TextAlignmentType.General);
    wb.Save(_destFilesPath + "example.xlsx");
}
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



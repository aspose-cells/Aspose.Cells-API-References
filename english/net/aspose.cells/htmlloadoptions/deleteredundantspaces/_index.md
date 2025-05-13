---
title: HtmlLoadOptions.DeleteRedundantSpaces
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether delete redundant spaces when the text wraps lines using br tag. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/deleteredundantspaces/
---
## HtmlLoadOptions.DeleteRedundantSpaces property

Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag. The default value is false.

```csharp
public bool DeleteRedundantSpaces { get; set; }
```

### Examples

```csharp
// Called: opts.DeleteRedundantSpaces = true;
public void HtmlLoadOptions_Property_DeleteRedundantSpaces()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"JAVA42797/";

    String html = "<p><i>Some text</i></p>";
    HtmlLoadOptions opts = new HtmlLoadOptions();
    opts.AutoFitColsAndRows = true;
    opts.DeleteRedundantSpaces = true;
    byte[] btsHtml = UTF8Encoding.UTF8.GetBytes(html);
    MemoryStream stream = new MemoryStream(btsHtml);
    // Create workbook from HTML string
    Workbook wb = new Workbook(stream, opts);
    Assert.AreEqual(wb.Worksheets[0].Cells["A1"].GetStyle().Font.IsItalic, true);
    wb.Save(CreateFolder(filePath) + "out.xlsx");
}
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



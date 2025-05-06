---
title: Font.Underline
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets or sets the font underline type
type: docs
url: /net/aspose.cells/font/underline/
---
## Font.Underline property

Gets or sets the font underline type.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(wb.Worksheets[1].Cells[&amp;quot;B1&amp;quot;].GetStyle().Font.Underline, FontUnderlineType.None);
[Test]
        public void Property_Underline()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-45582.xlsx&quot;);
            wb.Save(_destFilesPath + &quot;CELLSJAVA-45582.html&quot;, new HtmlSaveOptions());
            wb = new Workbook(_destFilesPath + &quot;CELLSJAVA-45582.html&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;Q17&quot;].GetStyle().Font.Underline, FontUnderlineType.None);
            Assert.AreEqual(wb.Worksheets[1].Cells[&quot;A1&quot;].GetStyle().Font.Underline, FontUnderlineType.Single);
            Assert.AreEqual(wb.Worksheets[1].Cells[&quot;B1&quot;].GetStyle().Font.Underline, FontUnderlineType.None);
        }
```

### See Also

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



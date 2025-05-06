---
title: HtmlSaveOptions.HideOverflowWrappedText
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Indicates whether to hide overflow text when the cell format is set to wrap text. The default value is false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Examples

```csharp
// Called: saveOptions.HideOverflowWrappedText = true;
[Test]
        public void Property_HideOverflowWrappedText()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-45899.xlsx&quot;);
            Style style= wb.CreateStyle();
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            style.IsTextWrapped=true;
            wb.Worksheets[0].Cells.ApplyStyle(style, flag);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            wb.Save(_destFilesPath + &quot;CELLSJAVA-45899.html&quot;, saveOptions);
            string text = File.ReadAllText(_destFilesPath + &quot;CELLSJAVA-45899.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;overflow:hidden;white-space:nowrap;&apos;&gt;（供来访客户推荐）注&quot;) &gt; -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



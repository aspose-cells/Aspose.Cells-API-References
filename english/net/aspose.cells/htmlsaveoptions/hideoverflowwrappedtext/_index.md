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
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSJAVA-45899.xlsx");
            Style style= wb.CreateStyle();
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            style.IsTextWrapped=true;
            wb.Worksheets[0].Cells.ApplyStyle(style, flag);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            wb.Save(_destFilesPath + "CELLSJAVA-45899.html", saveOptions);
            string text = File.ReadAllText(_destFilesPath + "CELLSJAVA-45899.html");
            Assert.IsTrue(text.IndexOf("overflow:hidden;white-space:nowrap;'>（供来访客户推荐）注") > -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



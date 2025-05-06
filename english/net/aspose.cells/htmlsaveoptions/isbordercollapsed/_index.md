---
title: HtmlSaveOptions.IsBorderCollapsed
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether the table borders are collapsed. The default value is true
type: docs
url: /net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

Indicates whether the table borders are collapsed. The default value is true.

```csharp
public bool IsBorderCollapsed { get; set; }
```

### Examples

```csharp
// Called: saveOptions.IsBorderCollapsed = false;
[Test]
        public void Property_IsBorderCollapsed()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSNET-56447.xlsx&quot;);
            var docCulture = new System.Globalization.CultureInfo(&quot;de-DE&quot;);
            Thread.CurrentThread.CurrentCulture = docCulture;
            Thread.CurrentThread.CurrentUICulture = docCulture;
            wb.Settings.CultureInfo = docCulture;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;
            wb.Save(_destFilesPath + &quot;CELLSNET-56447.html&quot;, saveOptions);
            string text = File.ReadAllText(_destFilesPath + &quot;CELLSNET-56447.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;transform:skew(-45deg) translateX(116.625pt)&quot;) &gt; -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



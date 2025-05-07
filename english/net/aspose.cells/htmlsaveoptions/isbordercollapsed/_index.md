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
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-56447.xlsx");
            var docCulture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = docCulture;
            Thread.CurrentThread.CurrentUICulture = docCulture;
            wb.Settings.CultureInfo = docCulture;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;
            wb.Save(_destFilesPath + "CELLSNET-56447.html", saveOptions);
            string text = File.ReadAllText(_destFilesPath + "CELLSNET-56447.html");
            Assert.IsTrue(text.IndexOf("transform:skew(-45deg) translateX(116.625pt)") > -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



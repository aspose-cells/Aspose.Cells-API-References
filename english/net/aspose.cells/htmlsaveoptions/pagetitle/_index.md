---
title: HtmlSaveOptions.PageTitle
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. The title of the html page. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/pagetitle/
---
## HtmlSaveOptions.PageTitle property

The title of the html page. Only for saving to html stream.

```csharp
public string PageTitle { get; set; }
```

### Examples

```csharp
// Called: saveOptions.PageTitle = &amp;quot;Excel1&amp;quot;;
[Test, Description(&quot;HtmlSaveOptions.PageTitle property need be checked by Manual&quot;)]
        public void Property_PageTitle()
        {
            string file = Constants.bugFilePath + &quot;savetest.xls&quot;;
            Workbook workbook = new Workbook(file);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.PageTitle = &quot;Excel1&quot;;
            FileStream fout = new FileStream(Constants.checkPath + &quot;HtmlSaveOptions_PageTitle_004.html&quot;, FileMode.Create);
            workbook.Save(fout, saveOptions);
            fout.Flush();
            fout.Close();
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



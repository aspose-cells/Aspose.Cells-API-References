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
// Called: saveOptions.PageTitle = "!1wrr$%&*-hewet1313";
[Test, Description("HtmlSaveOptions.PageTitle property need be checked by Manual")]
        public void Property_PageTitle()
        {
            string file = Constants.bugFilePath + "savetest.xls";
            Workbook workbook = new Workbook(file);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.PageTitle = "!1wrr$%&*-hewet1313";
            workbook.Save(Constants.checkPath + "HtmlSaveOptions_PageTitle_002.html", saveOptions);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



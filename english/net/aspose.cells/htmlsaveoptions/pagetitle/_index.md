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
// Called: saveOptions.PageTitle = "the Page Title";
public void HtmlSaveOptions_Property_PageTitle()
{
    Console.WriteLine("TEST_HtmlStreamSpecifyDir()");
    string infn = path + "TEST_HtmlStreamSpecifyDir.xlsx";
    string outfn = Constants.destPath + "TEST_HtmlStreamSpecifyDir_out.htm";
    Workbook book = new Workbook(infn);
    HtmlSaveOptions saveOptions = new HtmlSaveOptions();
    saveOptions.PageTitle = "the Page Title";
    saveOptions.AttachedFilesDirectory = Constants.destPath + @"TEST_HtmlStreamSpecifyDir_outDir";
    saveOptions.AttachedFilesUrlPrefix = @"http://www.example.com/usereport10_Attached/";
    FileStream fs = new FileStream(outfn, FileMode.OpenOrCreate);
    book.Save(fs,saveOptions);
    fs.Close();
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



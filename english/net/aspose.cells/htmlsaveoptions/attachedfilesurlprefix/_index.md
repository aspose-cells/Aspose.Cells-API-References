---
title: HtmlSaveOptions.AttachedFilesUrlPrefix
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Examples

```csharp
// Called: saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";
[Test, Description("HtmlSaveOptions.AttachedFilesUrlPrefix property need be checked by Manual")]
        public void HtmlSaveOptions_Property_AttachedFilesUrlPrefix()
        {
            string file = Constants.sourcePath + "TestWorkbook\\savetest.xls";
            Workbook workbook = new Workbook(file);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";
            FileStream fout = new FileStream(Constants.checkPath + "example.html", FileMode.Create);
            workbook.Save(fout, saveOptions);
            fout.Flush();
            fout.Close();
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



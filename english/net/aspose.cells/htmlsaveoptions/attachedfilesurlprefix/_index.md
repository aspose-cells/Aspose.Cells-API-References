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
// Called: saveOptions.AttachedFilesUrlPrefix = Constants.destPath;
[Test, Description("HtmlSaveOptions.AttachedFilesUrlPrefix property need be checked by Manual")]
        public void Property_AttachedFilesUrlPrefix()
        {
            string file = Constants.sourcePath + "TestWorkbook\\savetest.xls";
            Workbook workbook = new Workbook(file);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = Constants.destPath;
            FileStream fout = new FileStream(Constants.checkPath + "HtmlSaveOptions_AttachedFilesUrlPrefix_002.html", FileMode.Create);
            workbook.Save(fout, saveOptions);
            fout.Flush();
            fout.Close();
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



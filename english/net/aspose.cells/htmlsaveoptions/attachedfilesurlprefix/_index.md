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
// Called: saveopt.AttachedFilesUrlPrefix = &amp;quot;Test_HtmlToStreamIssue_AttachFileUrlPrefix_2&amp;quot;;
[Test]
        // http://www.aspose.com/community/forums/thread/250587.aspx
        public void Property_AttachedFilesUrlPrefix()
        {
            Console.WriteLine(&quot;Property_AttachedFilesUrlPrefix()&quot;);
            string infn = path + &quot;Test_HtmlToStreamIssue.xls&quot;;
            string outfn = Constants.destPath + &quot;Test_HtmlToStreamIssue_out.htm&quot;;
            string infn2 = path + &quot;Test_HtmlToStreamIssue_2.xls&quot;;
            string outfn2 = Constants.destPath + &quot;Test_HtmlToStreamIssue_2_out.htm&quot;;

            Workbook w = new Workbook(infn, new LoadOptions(LoadFormat.Excel97To2003));

            HtmlSaveOptions saveopt = new HtmlSaveOptions(SaveFormat.Html);
            saveopt.AttachedFilesDirectory = Constants.destPath + &quot;Test_HtmlToStreamIssue_AttachFileDir&quot;;
            saveopt.AttachedFilesUrlPrefix = &quot;Test_HtmlToStreamIssue_AttachFileUrlPrefix&quot;;
            saveopt.PageTitle = &quot;Test_HtmlToStreamIssue_title&quot;;

            FileStream fOut = new FileStream(outfn, FileMode.Create);
            w.Save(fOut, saveopt);
            fOut.Flush();
            fOut.Close();

            w = new Workbook(infn2, new LoadOptions(LoadFormat.Excel97To2003));
            saveopt = new HtmlSaveOptions(SaveFormat.Html);
            saveopt.AttachedFilesDirectory = Constants.destPath + &quot;Test_HtmlToStreamIssue_AttachFileDir_2&quot;;
            saveopt.AttachedFilesUrlPrefix = &quot;Test_HtmlToStreamIssue_AttachFileUrlPrefix_2&quot;;
            saveopt.PageTitle = &quot;Test_HtmlToStreamIssue_title_2&quot;;
            fOut = new FileStream(outfn2, FileMode.Create);
            w.Save(fOut, saveopt);
            fOut.Flush();
            fOut.Close();
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



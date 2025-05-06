---
title: HtmlSaveOptions.IsFullPathLink
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether using full path link in sheet00x.htmfilelist.xml and tabstrip.htm. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Examples

```csharp
// Called: options.IsFullPathLink = true;
[Test]
        public void Property_IsFullPathLink()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA43533/&quot;;
            string savePath = CreateFolder(filePath);

            Workbook workbook = new Workbook(filePath + &quot;TestAspose.xlsx&quot;);
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = true;
            options.StreamProvider = new ExportStreamProvider(savePath + @&quot;output\&quot;);

            FileStream outStream = new FileStream(savePath + &quot;out.html&quot;, FileMode.Create);
            workbook.Save(outStream, options);

        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



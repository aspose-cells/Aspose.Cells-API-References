---
title: HtmlSaveOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. If not setuse Encoding.UTF8 as default enconding type
type: docs
url: /net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

If not set,use Encoding.UTF8 as default enconding type.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: saveOps.Encoding = Encoding.UTF8;
[Test]
        public void Property_Encoding()
        {
            String filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41928/&quot;;

            string savePath = CreateFolder(filePath);
            Workbook book = new Workbook(filePath + &quot;diagramTest.xlsx&quot;);
            book.Save(savePath + &quot;out.html&quot;);

            FileStream baos = File.OpenWrite(savePath + &quot;stream.html&quot;);

            for (int i = 0; i &lt; book.Worksheets.Count; i++)
            {
                // only one page for test
                if (i != 0)
                {
                    book.Worksheets[i].IsVisible = false;
                }
            }
            HtmlSaveOptions saveOps = new HtmlSaveOptions();
            saveOps.ClearData = false;
            saveOps.CreateDirectory = false;
            saveOps.IsExpImageToTempDir = false;
            saveOps.ExportActiveWorksheetOnly = false;
            saveOps.ExportHiddenWorksheet = false;
            saveOps.ParseHtmlTagInCell = true;
            saveOps.Encoding = Encoding.UTF8;
            saveOps.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;
            saveOps.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            saveOps.ExportImagesAsBase64 = false;
            saveOps.AttachedFilesDirectory = CreateFolder(filePath + &quot;aaa&quot;);

            saveOps.StreamProvider = new JAVA41928StreamProvider(CreateFolder(filePath + &quot;aaa&quot;));
            book.Save(baos, saveOps);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: HtmlSaveOptions.ExportCommentsType
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Represents type of exporting comments to html files
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Represents type of exporting comments to html files.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportCommentsType = PrintCommentsType.PrintSheetEnd;
[Test]
        public void Property_ExportCommentsType()
        {
            Workbook wb = new Aspose.Cells.Workbook(Constants.HtmlPath + &quot;CELLSNET-55893.xlsx&quot;);
            wb.Worksheets.ActiveSheetIndex = 1;
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportActiveWorksheetOnly = true; 
            saveOptions.IsExportComments = true;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintSheetEnd;
            wb.Save(_destFilesPath + &quot;CELLSNET-55893.html&quot;, saveOptions);
            string text = File.ReadAllText(_destFilesPath + &quot;CELLSNET-55893.html&quot;);
            int n1 = text.IndexOf(&quot;&lt;div id = &apos;Comment_1_1&apos; style=&apos;text-align:left;&apos;&quot;);
            int n2 = text.IndexOf(&quot;&lt;div id = &apos;Comment_1_2&apos; style=&apos;text-align:left;&apos;&quot;);
            int n3 = text.IndexOf(&quot;&lt;div id = &apos;Comment_1_3&apos; style=&apos;text-align:left;&apos;&quot;);
            int n4 = text.IndexOf(&quot;&lt;div id = &apos;Comment_1_4&apos; style=&apos;text-align:left;&apos;&quot;);
            Assert.IsTrue(-1 &lt; n1 &amp;&amp; n1 &lt; n2 &amp;&amp; n2 &lt; n3 &amp;&amp; n3 &lt; n4);
        }
```

### See Also

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



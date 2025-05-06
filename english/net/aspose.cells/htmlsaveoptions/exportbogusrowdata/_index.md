---
title: HtmlSaveOptions.ExportBogusRowData
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel please keep the default value
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportbogusrowdata/
---
## HtmlSaveOptions.ExportBogusRowData property

Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.

```csharp
public bool ExportBogusRowData { get; set; }
```

### Examples

```csharp
// Called: saveOptions.ExportBogusRowData = true;
[Test]
        public void Property_ExportBogusRowData()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA41169/&quot;;

            Workbook workbook = new Workbook(filePath + &quot;sample2.xlsx&quot;);
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportBogusRowData = false;
            workbook.Save(Constants.destPath + &quot;JAVA41169.html&quot;, saveOptions);
           string text = File.ReadAllText(Constants.destPath + &quot;JAVA41169.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;&lt;![if supportMisalignedColumns]&gt;&quot;) == -1);
            saveOptions.ExportBogusRowData = true;
            workbook.Save(Constants.destPath + &quot;JAVA41169_1.html&quot;, saveOptions);
            text = File.ReadAllText(Constants.destPath + &quot;JAVA41169_1.html&quot;);
            Assert.IsTrue(text.IndexOf(&quot;&lt;![if supportMisalignedColumns]&gt;&quot;) != -1);
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



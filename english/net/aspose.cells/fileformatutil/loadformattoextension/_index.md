---
title: FileFormatUtil.LoadFormatToExtension
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converts a load format enumerated value into a file extension
type: docs
url: /net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Converts a load format enumerated value into a file extension.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loaded file format. |

### Return Value

The returned extension is a lower-case string with a leading dot.

### Remarks

If it can not be converted, returns null.

### Examples

```csharp
// Called: suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx);
[Test]
        public void Method_LoadFormat_()
        {
            //The annotated test code is currently not supported

            string suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto);
            Assert.AreEqual(null, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv);
            Assert.AreEqual(&quot;.csv&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003);
            Assert.AreEqual(&quot;.xls&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx);
            Assert.AreEqual(&quot;.xlsx&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv);
            Assert.AreEqual(&quot;.txt&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.TabDelimited);
            Assert.AreEqual(&quot;.txt&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods);
            Assert.AreEqual(&quot;.ods&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.SpreadsheetML);
            Assert.AreEqual(&quot;.xml&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb);
            Assert.AreEqual(&quot;.xlsb&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Numbers);
            Assert.AreEqual(&quot;.numbers&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Fods);
            Assert.AreEqual(&quot;.fods&quot;, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Image);
            Assert.AreEqual(null, suffix);

            suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Unknown);
            Assert.AreEqual(null, suffix);

            
            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Ots);
            //Assert.AreEqual(&quot;.ots&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Xml);
            //Assert.AreEqual(&quot;.xml&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Epub);
            //Assert.AreEqual(&quot;.epub&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Azw3);
            //Assert.AreEqual(&quot;.azw3&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Html);
            //Assert.AreEqual(&quot;.html&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.MHtml);
            //Assert.AreEqual(&quot;.mhtml&quot;, suffix);


            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Sxc);
            //Assert.AreEqual(&quot;.sxc&quot;, suffix);

            //suffix = FileFormatUtil.LoadFormatToExtension(LoadFormat.Json);
            //Assert.AreEqual(&quot;.json&quot;, suffix);


        }
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: HtmlLoadOptions.SupportDivTag
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether support the layout of div tag when the html file contains it. The default value is false
type: docs
url: /net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Indicates whether support the layout of `<div>` tag when the html file contains it. The default value is false.

```csharp
public bool SupportDivTag { get; set; }
```

### Examples

```csharp
// Called: options.SupportDivTag = true;
[Test]
        public void Property_SupportDivTag()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET44699And44700And44701/&quot;;

            string savePath = CreateFolder(filePath);
            HtmlLoadOptions options = new HtmlLoadOptions();
            options.SupportDivTag = true;
            Workbook wb = null;
            wb = new Workbook(filePath + &quot;sample1.html&quot;, options);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;This is a div with display set to none&quot;);
            Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
            wb.Save(savePath + &quot;out1.xlsx&quot;);

            wb = new Workbook(filePath + &quot;sample2.html&quot;, options);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;This is a div with display set to block&quot;);
            Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
            wb.Save(savePath + &quot;out2.xlsx&quot;);

            wb = new Workbook(filePath + &quot;sample3.html&quot;, options);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;This is just a plain div&quot;);
            Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
            wb.Save(savePath + &quot;out3.xlsx&quot;);

            wb = new Workbook(filePath + &quot;pre.html&quot;, options);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;This is hidden&quot;);
            Assert.Greater(wb.Worksheets[0].Cells.Rows[0].Height, 0);
            wb.Save(savePath + &quot;pre.xlsx&quot;);
        }
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



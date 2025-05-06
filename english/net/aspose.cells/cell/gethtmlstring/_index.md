---
title: Cell.GetHtmlString
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the html string which contains data and some formats in this cell
type: docs
url: /net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Gets the html string which contains data and some formats in this cell.

```csharp
public string GetHtmlString(bool html5)
```

| Parameter | Type | Description |
| --- | --- | --- |
| html5 | Boolean | Indicates whether the value is compatible for html5 |

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;&amp;lt;div&amp;gt;&amp;lt;span Style=\&amp;quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&amp;quot;&amp;gt;asd&amp;lt;/span&amp;gt;&amp;lt;span Style=\&amp;quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\&amp;quot;&amp;gt;fasdf&amp;lt;/span&amp;gt;&amp;lt;span Style=\&amp;quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&amp;quot;&amp;gt;sdf&amp;lt;/span&amp;gt;&amp;lt;/div&amp;gt;&amp;quot;, cell.GetHtmlString(true));
[Test]
        public void Method_Boolean_()
        {


            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-42528.xlsx&quot;);
            Cell cell = wb.Worksheets[0].Cells[&quot;B2&quot;];
            Assert.AreEqual(&quot;&lt;Font Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&quot;&gt;asd&lt;/Font&gt;&lt;Font Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\&quot;&gt;fasdf&lt;/Font&gt;&lt;Font Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&quot;&gt;sdf&lt;/Font&gt;&quot;, cell.HtmlString);
            Assert.AreEqual(&quot;&lt;div&gt;&lt;span Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&quot;&gt;asd&lt;/span&gt;&lt;span Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #ff0000;VERTICAL-ALIGN: bottom;\&quot;&gt;fasdf&lt;/span&gt;&lt;span Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&quot;&gt;sdf&lt;/span&gt;&lt;/div&gt;&quot;, cell.GetHtmlString(true));
            Assert.AreEqual(&quot;&lt;Font Style=\&quot;FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #000000;VERTICAL-ALIGN: bottom;\&quot;&gt;&lt;/Font&gt;&quot;, wb.Worksheets[0].Cells[&quot;A1&quot;].HtmlString);
            wb.Save(Constants.destPath + &quot;CELLSJAVA42528.html&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



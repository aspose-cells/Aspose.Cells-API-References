---
title: Cell.HtmlString
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the html string which contains data and some formats in this cell
type: docs
url: /net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Gets and sets the html string which contains data and some formats in this cell.

```csharp
public string HtmlString { get; set; }
```

### Examples

```csharp
// Called: cell.HtmlString = &amp;quot;&amp;lt;p&amp;gt;&amp;lt;span style=\&amp;quot;font-size:smaller\&amp;quot;&amp;gt;Details:&amp;lt;/span&amp;gt;&amp;lt;/p&amp;gt; &amp;lt;p&amp;gt;7:00AM-3:00PM&amp;lt;/p&amp;gt; &amp;lt;p&amp;gt;STARTING DATE: September 5th, 2017&amp;lt;/p&amp;gt;&amp;quot;;
[Test]
        public void Property_HtmlString()
        {
            Workbook wb = new Workbook();

            Worksheet ws = wb.Worksheets[0];

            Cell cell = ws.Cells[&quot;C4&quot;];
            cell.HtmlString = &quot;&lt;p&gt;&lt;span style=\&quot;font-size:smaller\&quot;&gt;Details:&lt;/span&gt;&lt;/p&gt; &lt;p&gt;7:00AM-3:00PM&lt;/p&gt; &lt;p&gt;STARTING DATE: September 5th, 2017&lt;/p&gt;&quot;;

            wb.Save(Constants.destPath + &quot;CellsNet45817.xlsx&quot;);
            
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



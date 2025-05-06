---
title: Hyperlink.Delete
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink method. Deletes this hyperlink
type: docs
url: /net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Deletes this hyperlink

```csharp
public void Delete()
```

### Examples

```csharp
// Called: hyperlink.Delete();
[Test]
        public void Method_Delete()
        {
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            loadOpts.Region = CountryCode.USA;
            Workbook wb = new Workbook(Constants.HtmlPath + &quot;CELLSJAVA-45701.html&quot;, loadOpts);
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i &lt; ws.Hyperlinks.Count; i++)
            {
                Hyperlink hyperlink = ws.Hyperlinks[i];
                hyperlink.Delete();
            }
            Aspose.Cells.Font font = ws.Cells[&quot;A14&quot;].GetStyle().Font;
            Assert.AreEqual(&quot;Arial&quot;, font.Name);
            Assert.AreEqual(10, font.Size);
            Assert.IsFalse(font.IsItalic);
            CompareColor.compare(&quot;A14&quot;, Color.FromArgb(255, 0, 0, 0), font.Color);
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: Cell.IsRichText
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Indicates whether the string value of this cell is a rich formatted text
type: docs
url: /net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Indicates whether the string value of this cell is a rich formatted text.

```csharp
public bool IsRichText()
```

### Examples

```csharp
// Called: Assert.AreEqual(cells[&amp;quot;A2&amp;quot;].IsRichText(), true);
[Test]
        public void Method_IsRichText()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET44336/&quot;;

            HtmlLoadOptions opts = new HtmlLoadOptions(LoadFormat.Html);
            opts.Encoding = Encoding.UTF8;

            Workbook workbook = new Workbook(filePath + &quot;test.html&quot;, opts);
            Cells cells = workbook.Worksheets[0].Cells;
            if (cells[&quot;A1&quot;].IsRichText())
            {
                Assert.AreEqual(cells[&quot;A1&quot;].GetCharacters().Length, 1);
            }
            //Assert.AreEqual(cells[&quot;A1&quot;].IsRichText(), false);

            Assert.AreEqual(cells[&quot;A1&quot;].GetStyle().Font.Color, Color.FromArgb(255, 147, 35, 32));

            Assert.AreEqual(cells[&quot;A2&quot;].IsRichText(), true);
            Assert.AreEqual(cells[&quot;A2&quot;].GetCharacters()[0].Font.Color, Color.FromArgb(255, 147, 35, 32));
            Assert.AreEqual(cells[&quot;A2&quot;].GetCharacters()[1].Font.Color, Color.FromArgb(255, 30, 127, 153));

            if (cells[&quot;A3&quot;].IsRichText())
            {
                Assert.AreEqual(cells[&quot;A3&quot;].GetCharacters().Length, 1);
            }
            //Assert.AreEqual(cells[&quot;A3&quot;].IsRichText(), false);
            Assert.AreEqual(cells[&quot;A3&quot;].GetStyle().Font.Color, Color.FromArgb(255, 0, 0, 0));

            workbook.Save(CreateFolder(filePath) + &quot;output.xlsx&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



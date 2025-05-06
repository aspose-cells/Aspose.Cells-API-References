---
title: Style.QuotePrefix
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the cells value starts with single quote mark
type: docs
url: /net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indicates whether the cell's value starts with single quote mark.

```csharp
public bool QuotePrefix { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workBook.Worksheets[0].Cells[&amp;quot;B10&amp;quot;].GetStyle().QuotePrefix);
[Test]
        public void Property_QuotePrefix()
        {

            var workBook = new Workbook(Constants.sourcePath + &quot;CELLSNET45504.xml&quot;);
            // workBook.Worksheets[0].Charts.Clear();
            Assert.IsTrue(workBook.Worksheets[0].Cells[&quot;B10&quot;].GetStyle().QuotePrefix);
            workBook.Save(Constants.destPath + &quot;CELLSNET45504.xml&quot;);
            workBook = new Workbook(Constants.destPath + &quot;CELLSNET45504.xml&quot;);
            Assert.IsTrue(workBook.Worksheets[0].Cells[&quot;B10&quot;].GetStyle().QuotePrefix);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



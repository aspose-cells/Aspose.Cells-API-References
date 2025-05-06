---
title: Range.RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets the ranges refers to
type: docs
url: /net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Gets the range's refers to.

```csharp
public string RefersTo { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;=Sheet1!$G$4:$H$6&amp;quot;, ranges[0].RefersTo);
[Test]
        public void Property_RefersTo()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CELLSNET48628.xlsx&quot;);
            book.Save(Constants.destPath + @&quot;CELLSNET48623.ods&quot;);
            book = new Workbook(Constants.destPath + @&quot;CELLSNET48623.ods&quot;);
            Name name = book.Worksheets.Names[&quot;abc&quot;];
            Aspose.Cells.Range[] ranges = name.GetRanges();
            Assert.AreEqual(&quot;=Sheet1!$G$4:$H$6&quot;, ranges[0].RefersTo);
            Assert.AreEqual(&quot;=Sheet1!$J$8:$K$10&quot;, ranges[1].RefersTo);
            Assert.AreEqual(&quot;=SUM((A1,A5,A9))&quot;, book.Worksheets[0].Cells[&quot;F8&quot;].Formula);
           
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



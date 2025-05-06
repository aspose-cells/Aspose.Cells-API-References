---
title: Range.Address
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets address of the range
type: docs
url: /net/aspose.cells/range/address/
---
## Range.Address property

Gets address of the range.

```csharp
public string Address { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.Ranges[0].Address, &amp;quot;B1:C1&amp;quot;);
[Test]
        public void Property_Address()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Aspose.Cells.Range r1 = cells.CreateRange(&quot;B1:C10&quot;);
            Aspose.Cells.Range r2 = cells.CreateRange(&quot;C2:D10&quot;);
            UnionRange r = r1.UnionRanges(new Aspose.Cells.Range[] { r2 });
            Assert.AreEqual(r.RangeCount, 2);
            Assert.AreEqual(r.Ranges[0].Address, &quot;B1:C1&quot;);
            Assert.AreEqual(r.Ranges[1].Address, &quot;B2:D10&quot;);
            //Excel&apos;s VBA does not do in this way, if those ranges cannot be unioned completely, VBA just do nothing
            //The result of below VBA code is $B$1:$C$10 and $C$2:$D$10
            //Dim r As Range
            //Set r = Union(Range(&quot;B1:C10&quot;), Range(&quot;C2:D10&quot;))
            //Let sn = 1
            //Dim r2 As Range
            //For Each r2 In r.Areas
            //    Range(&quot;A&quot; &amp; sn).Value = r2.Address
            //    sn = sn + 1
            //Next r2
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



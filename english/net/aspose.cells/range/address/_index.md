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
// Called: Assert.AreEqual(r.Ranges[1].Address, "B2:D10");
[Test]
        public void Property_Address()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Aspose.Cells.Range r1 = cells.CreateRange("B1:C10");
            Aspose.Cells.Range r2 = cells.CreateRange("C2:D10");
            UnionRange r = r1.UnionRanges(new Aspose.Cells.Range[] { r2 });
            Assert.AreEqual(r.RangeCount, 2);
            Assert.AreEqual(r.Ranges[0].Address, "B1:C1");
            Assert.AreEqual(r.Ranges[1].Address, "B2:D10");
            //Excel's VBA does not do in this way, if those ranges cannot be unioned completely, VBA just do nothing
            //The result of below VBA code is $B$1:$C$10 and $C$2:$D$10
            //Dim r As Range
            //Set r = Union(Range("B1:C10"), Range("C2:D10"))
            //Let sn = 1
            //Dim r2 As Range
            //For Each r2 In r.Areas
            //    Range("A" & sn).Value = r2.Address
            //    sn = sn + 1
            //Next r2
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



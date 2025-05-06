---
title: ReferredAreaCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ReferredAreaCollection property. 
type: docs
url: /net/aspose.cells/referredareacollection/item/
---
## ReferredAreaCollection indexer

```csharp
public ReferredArea this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index |  |

### Examples

```csharp
// Called: ReferredArea ra = worksheet1.Cells[&amp;quot;A1&amp;quot;].GetPrecedents()[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add(&quot;Sheet2&quot;);
            Worksheet worksheet1 = workbook.Worksheets[&quot;Sheet1&quot;];
            // the named range
            workbook.Worksheets[&quot;Sheet2&quot;].Cells.CreateRange(&quot;E5:I6&quot;).Name = &quot;someNamedRange_1&quot;;
            worksheet1.Cells[&quot;A1&quot;].Formula = &quot;=SUM(someNamedRange_1)&quot;;
            ReferredArea ra = worksheet1.Cells[&quot;A1&quot;].GetPrecedents()[0];
            Assert.AreEqual(&quot;Sheet2&quot;, ra.SheetName, &quot;Precedent&apos;s referred sheet&quot;);
        }
```

### See Also

* class [ReferredArea](../../referredarea/)
* class [ReferredAreaCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



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
// Called: ReferredArea ra = worksheet1.Cells["A1"].GetPrecedents()[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets["Sheet1"];
            // the named range
            workbook.Worksheets["Sheet2"].Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
            worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
            ReferredArea ra = worksheet1.Cells["A1"].GetPrecedents()[0];
            Assert.AreEqual("Sheet2", ra.SheetName, "Precedent's referred sheet");
        }
```

### See Also

* class [ReferredArea](../../referredarea/)
* class [ReferredAreaCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



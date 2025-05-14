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
// Called: Assert.AreEqual("Sheet2", prec[0].SheetName);
public void ReferredAreaCollection_Property_Item()
{
    Workbook wb = new Workbook();
    wb.Worksheets.Add("Sheet2");
    var worksheet1 = wb.Worksheets["Sheet1"];
    // the named range 
    wb.Worksheets["Sheet2"].Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
    worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
    var prec = worksheet1.Cells["A1"].GetPrecedents();
    Assert.AreEqual("Sheet2", prec[0].SheetName);
}
```

### See Also

* class [ReferredArea](../../referredarea/)
* class [ReferredAreaCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



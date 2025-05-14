---
title: Range.Item
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets Cell object in this range
type: docs
url: /net/aspose.cells/range/item/
---
## Range indexer

Gets [`Cell`](../../cell/) object in this range.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parameter | Description |
| --- | --- |
| rowOffset | Row offset in this range, zero based. |
| columnOffset | Column offset in this range, zero based. |

### Return Value

[`Cell`](../../cell/) object.

### Examples

```csharp
// Called: Assert.AreEqual(rng[0,0].StringValue, "Id");
public void Range_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    DataTable dt = CreateValidTable1();

    Aspose.Cells.Range rng = GetRange(workbook, "Fact_ContractId", true);
    InsertRange_1(workbook, rng, dt);

    Assert.AreEqual(rng[0,0].StringValue, "Id");
    rng = GetRange(workbook, "Fact_MeasureValue", true);
    InsertRange_1(workbook, rng, dt);
    string output = Constants.destPath + "example.xlsx";
    workbook.Save(output);
    Assert.AreEqual(workbook.Worksheets["Facts"].Cells["A6"].StringValue, "Id");
    Assert.AreEqual(workbook.Worksheets["Facts"].Cells["A7"].StringValue, "1001");
   AssertHelper.AreEqual(workbook.Worksheets["Facts"].Cells["A3"].GetStyle().ForegroundColor, Color.Red);
   AssertHelper.AreEqual(workbook.Worksheets["Facts"].Cells["A6"].GetStyle().ForegroundColor, Color.FromArgb(0,176,80));
           
            
}
```

### See Also

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



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
// Called: Assert.AreEqual("1:1", range.EntireRow.Address);
public void Range_Property_Address()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Aspose.Cells.Range range = cells.CreateRange("A1");
    Assert.AreEqual("A1", range.Address);
    Assert.AreEqual("B2", range.GetOffset(1, 1).Address);
    Assert.AreEqual("1:1", range.EntireRow.Address);
    Assert.AreEqual("A:A", range.EntireColumn.Address);
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



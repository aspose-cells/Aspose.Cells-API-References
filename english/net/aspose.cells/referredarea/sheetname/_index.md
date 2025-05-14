---
title: ReferredArea.SheetName
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates which sheet this reference is in
type: docs
url: /net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indicates which sheet this reference is in.

```csharp
public string SheetName { get; }
```

### Remarks

If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Examples

```csharp
// Called: Assert.AreEqual("Sheet2", ra.SheetName, "Precedent's referred sheet");
public void ReferredArea_Property_SheetName()
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

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



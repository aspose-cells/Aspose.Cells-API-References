---
title: Cell.DateTimeValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the DateTime value contained in the cell
type: docs
url: /net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Gets the DateTime value contained in the cell.

```csharp
public DateTime DateTimeValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(dt, cells["M16"].DateTimeValue);
public void Cell_Property_DateTimeValue()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.numbers");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("FROZEN TURKEYS", cells["A12"].StringValue);
    Assert.AreEqual(true, cells["A12"].GetStyle().Font.IsBold);
    Assert.AreEqual(true, cells["A12"].GetStyle().Font.IsItalic);
    DateTime dt = new DateTime(2023, 11, 13);
    Assert.AreEqual(dt, cells["M16"].DateTimeValue);
    dt = new DateTime(2023, 10, 19);
    Assert.AreEqual(dt, cells["B2"].DateTimeValue);
    //Assert.AreEqual("", cells["M16"].DateTimeValue);
    Assert.AreEqual("1.00", cells["G42"].StringValue);
    Assert.AreEqual("POULTRY", cells["A29"].StringValue);
    Assert.AreEqual("PORK", cells["A32"].StringValue);
    Assert.AreEqual("MISC.", cells["A52"].StringValue);
    Assert.AreEqual("FROZEN BUTTERBALL SMOKED TURKEY        (9.5-13LB. AVG) ", cells["B20"].StringValue);
    Assert.AreEqual("Account #", cells["I61"].StringValue);
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



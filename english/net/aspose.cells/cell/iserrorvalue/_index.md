---
title: Cell.IsErrorValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks if the value of this cell is an error
type: docs
url: /net/aspose.cells/cell/iserrorvalue/
---
## Cell.IsErrorValue property

Checks if the value of this cell is an error.

```csharp
public bool IsErrorValue { get; }
```

### Remarks

Also applies to formula cell to check whether the calculated result is an error.

### Examples

```csharp
// Called: Assert.IsTrue(cell.IsErrorValue, "Cell.IsErrorValue for SPILLERR");
public void Cell_Property_IsErrorValue()
{ //NEED TO IMPROVE corresponding apis and then UPDATE this case
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.EmbeddedImage = File.ReadAllBytes(Constants.sourcePath + "1.png");
    Assert.AreEqual("#VALUE!", cell.DisplayStringValue, "Cell.DisplayStringValue for SPILLERR");
    Assert.AreEqual("#VALUE!", cell.StringValue, "Cell.StringValue for EmbeddedImage");
    Assert.AreEqual("#VALUE!", cell.Value, "Cell.Value for EmbeddedImage"); //this may be changed in later versions
    Assert.IsFalse(cell.IsErrorValue, "Cell.IsErrorValue for EmbeddedImage");
    Assert.AreEqual(CellValueType.IsError, cell.Type, "Cell.Type for EmbeddedImage"); //this should fail
    cells[1, 0].PutValue("abc");
    cell.SetDynamicArrayFormula("=B1:B2", new FormulaParseOptions(), true);
    //Assert.AreEqual("#SPILL!", cell.DisplayStringValue, "Cell.DisplayStringValue for SPILLERR");
    Assert.AreEqual("#VALUE!", cell.StringValue, "Cell.StringValue for SPILLERR");
    Assert.AreEqual("#VALUE!", cell.Value, "Cell.Value for SPILLERR"); //this may be changed in later versions
    Assert.IsTrue(cell.IsErrorValue, "Cell.IsErrorValue for SPILLERR");
    Assert.AreEqual(CellValueType.IsError, cell.Type, "Cell.Type for SPILLERR");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



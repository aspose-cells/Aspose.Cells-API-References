---
title: Workbook.HasCustomFunction
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Detects whether there is custom function used in this workbook such as in cells formula in defined names
type: docs
url: /net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Detects whether there is custom function used in this workbook, such as in cell's formula, in defined names...

```csharp
public bool HasCustomFunction { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(wb.HasCustomFunction, "No custom function in Name");
public void Workbook_Property_HasCustomFunction()
{
    Workbook wb = new Workbook();
    NameCollection nc = wb.Worksheets.Names;
    nc[nc.Add("TestName1")].RefersTo = "=SUM(Sheet1!$C$1:$C$2)";
    Assert.IsFalse(wb.HasCustomFunction, "No custom function in Name");
    nc[nc.Add("TestName2")].RefersTo = "=MYTESTFUNC()";
    Assert.IsTrue(wb.HasCustomFunction, "Custom function in Name");

    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.Formula = "=ABS(C1)";
    Assert.IsFalse(cell.HasCustomFunction, "Fix function");
    cell.Formula = "=SUM(C1)";
    Assert.IsFalse(cell.HasCustomFunction, "Var function");
    cell.Formula = "=XLOOKUP(C1:C2,D1:D2,E1:E2)";
    Assert.IsFalse(cell.HasCustomFunction, "Future function");
    cell.Formula = "=MYTESTFUNC(C1)";
    Assert.IsTrue(cell.HasCustomFunction, "Custom function");
    cell.Formula = "=TestName2";
    Assert.IsTrue(cell.HasCustomFunction, "Using Name with custom function");
    cell.Formula = "=MYTESTFUNC(TestName2)";
    Assert.IsTrue(cell.HasCustomFunction, "Multiple occurences of Custom function");
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



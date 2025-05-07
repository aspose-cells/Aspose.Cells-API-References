---
title: Cell.HasCustomFunction
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks whether there is custom functionunsupported function in this cells formula
type: docs
url: /net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Checks whether there is custom function(unsupported function) in this cell's formula.

```csharp
public bool HasCustomFunction { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(cell.HasCustomFunction, "Fix function");
[Test]
        public void Property_HasCustomFunction()
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



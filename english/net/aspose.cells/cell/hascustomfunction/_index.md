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
// Called: Assert.IsTrue(cell.HasCustomFunction, &amp;quot;Multiple occurences of Custom function&amp;quot;);
[Test]
        public void Property_HasCustomFunction()
        {
            Workbook wb = new Workbook();
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add(&quot;TestName1&quot;)].RefersTo = &quot;=SUM(Sheet1!$C$1:$C$2)&quot;;
            Assert.IsFalse(wb.HasCustomFunction, &quot;No custom function in Name&quot;);
            nc[nc.Add(&quot;TestName2&quot;)].RefersTo = &quot;=MYTESTFUNC()&quot;;
            Assert.IsTrue(wb.HasCustomFunction, &quot;Custom function in Name&quot;);

            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.Formula = &quot;=ABS(C1)&quot;;
            Assert.IsFalse(cell.HasCustomFunction, &quot;Fix function&quot;);
            cell.Formula = &quot;=SUM(C1)&quot;;
            Assert.IsFalse(cell.HasCustomFunction, &quot;Var function&quot;);
            cell.Formula = &quot;=XLOOKUP(C1:C2,D1:D2,E1:E2)&quot;;
            Assert.IsFalse(cell.HasCustomFunction, &quot;Future function&quot;);
            cell.Formula = &quot;=MYTESTFUNC(C1)&quot;;
            Assert.IsTrue(cell.HasCustomFunction, &quot;Custom function&quot;);
            cell.Formula = &quot;=TestName2&quot;;
            Assert.IsTrue(cell.HasCustomFunction, &quot;Using Name with custom function&quot;);
            cell.Formula = &quot;=MYTESTFUNC(TestName2)&quot;;
            Assert.IsTrue(cell.HasCustomFunction, &quot;Multiple occurences of Custom function&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



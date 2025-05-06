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
// Called: Assert.IsFalse(wb.HasCustomFunction, &amp;quot;No custom function in Name&amp;quot;);
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

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



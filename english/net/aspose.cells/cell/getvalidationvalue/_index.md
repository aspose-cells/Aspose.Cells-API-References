---
title: Cell.GetValidationValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the value of validation which applied to this cell
type: docs
url: /net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Gets the value of validation which applied to this cell.

```csharp
public bool GetValidationValue()
```

### Examples

```csharp
// Called: Assert.IsTrue(cell.GetValidationValue(), &amp;quot;1 &amp;lt;C1(blank cell, IgnoreBlank)&amp;quot;);
[Test]
        public void Method_GetValidationValue()
        {
            Workbook wb = new Workbook();
            ValidationCollection vldts = wb.Worksheets[0].Validations;
            Validation vldt = vldts[vldts.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            vldt.IgnoreBlank = true;
            vldt.Type = ValidationType.WholeNumber;
            vldt.Operator = OperatorType.LessThan;
            vldt.Formula1 = &quot;=C1&quot;;
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            cell.PutValue(1);
            Assert.IsTrue(cell.GetValidationValue(), &quot;1 LessThan blank cell(IgnoreBlank)&quot;);
            cell.PutValue(true);
            Assert.IsTrue(cell.GetValidationValue(), &quot;TRUE LessThan blank cell(IgnoreBlank)&quot;);
            vldt.Operator = OperatorType.Between;
            vldt.Formula2 = &quot;=D1&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;TRUE Between blank cells(IgnoreBlank)&quot;);
            cells[0, 3].PutValue(1);
            Assert.IsTrue(cell.GetValidationValue(), &quot;TRUE Between blank and non blank(IgnoreBlank)&quot;);
            cell.PutValue(1);
            Assert.IsTrue(cell.GetValidationValue(), &quot;1 Between blank and non blank(IgnoreBlank)&quot;);
            cell.PutValue(2);
            Assert.IsTrue(cell.GetValidationValue(), &quot;2 Between blank and non blank(IgnoreBlank)&quot;);
            vldt.IgnoreBlank = false;
            Assert.IsFalse(cell.GetValidationValue(), &quot;2 Between blank and non blank(not IgnoreBlank)&quot;);
            cell.PutValue(1);
            Assert.IsTrue(cell.GetValidationValue(), &quot;1 Between blank and non blank(not IgnoreBlank)&quot;);
            cell.PutValue(0);
            Assert.IsTrue(cell.GetValidationValue(), &quot;0 Between blank and non blank(not IgnoreBlank)&quot;);
            cell.PutValue(-1);
            Assert.IsFalse(cell.GetValidationValue(), &quot;-1 Between blank and non blank(not IgnoreBlank)&quot;);

            vldt.Type = ValidationType.Custom;
            vldt.Formula1 = &quot;=C1&gt;A1&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;-1 &lt;C1(blank cell, not IgnoreBlank)&quot;);
            cell.PutValue(0);
            Assert.IsFalse(cell.GetValidationValue(), &quot;0 &lt;C1(blank cell, not IgnoreBlank)&quot;);
            vldt.IgnoreBlank = true;
            Assert.IsTrue(cell.GetValidationValue(), &quot;0 &lt;C1(blank cell, IgnoreBlank)&quot;);
            cell.PutValue(1);
            Assert.IsTrue(cell.GetValidationValue(), &quot;1 &lt;C1(blank cell, IgnoreBlank)&quot;);

            vldt.Formula1 = &quot;=C1-D1&gt;0&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;C1-D1&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=IF(TRUE,A1,C1)&gt;0&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;IF(TRUE,A1,C1)&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=IF(FALSE,A1,C1)&gt;0&quot;;
            Assert.IsFalse(cell.GetValidationValue(), &quot;IF(FALSE,A1,C1)&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=-C1&gt;0&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;-C1&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=ABS(C1)&gt;0&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;ABS(C1)&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=INDIRECT(\&quot;C1\&quot;)&gt;0&quot;;
            Assert.IsFalse(cell.GetValidationValue(), &quot;INDIRECT(\&quot;C1\&quot;)&gt;0(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=INDIRECT(\&quot;C1\&quot;)&quot;;
            Assert.IsFalse(cell.GetValidationValue(), &quot;INDIRECT(\&quot;C1\&quot;)(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=C1&gt;D1&quot;;
            Assert.IsTrue(cell.GetValidationValue(), &quot;C1&gt;D1(blank cell in formula, IgnoreBlank)&quot;);
            vldt.Formula1 = &quot;=SUM(C1)&gt;D1&quot;;
            Assert.IsFalse(cell.GetValidationValue(), &quot;SUM(C1)&gt;D1(blank cell in formula, IgnoreBlank)&quot;);

            vldt = vldts[vldts.Add(CellArea.CreateCellArea(2, 0, 2, 0))];
            vldt.Type = ValidationType.Custom;
            vldt.IgnoreBlank = true;
            vldt.Formula1 = &quot;=D1:D3&gt;0&quot;;
            cell = cells[2, 0];
            cell.PutValue(&quot;abc&quot;);
            Assert.IsTrue(cell.GetValidationValue(), &quot;D1:D3&gt;0(D1=1 and D3 is blank, IgnoreBlank)&quot;);
            cells[0, 3].PutValue(-1);
            Assert.IsFalse(cell.GetValidationValue(), &quot;D1:D3&gt;0(D1=-1 and D3 is blank, IgnoreBlank)&quot;);
            cells[2, 3].PutValue(1);
            Assert.IsFalse(cell.GetValidationValue(), &quot;D1:D3&gt;0(D1=-1 and D3=1, IgnoreBlank)&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



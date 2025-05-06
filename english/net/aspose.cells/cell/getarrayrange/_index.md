---
title: Cell.GetArrayRange
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the array range if the cells formula is an array formula
type: docs
url: /net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

Gets the array range if the cell's formula is an array formula.

```csharp
public CellArea GetArrayRange()
```

### Return Value

The array range.

### Remarks

Only applies when the cell's formula is an array formula

### Examples

```csharp
// Called: AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &amp;quot;.ArrayRange&amp;quot;);
[Test]
        public void Method_GetArrayRange()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            string fml = &quot;=LET(x,{1,2,3},SUM(x))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            CellArea expected = CellArea.CreateCellArea(0, 0, 0, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;6&quot;, }, cells, expected, fml);

            fml = &quot;=LET(x,{1,2,3},ABS(x))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 0, 2);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;1&quot;, &quot;2&quot;, &quot;3&quot; }, cells, expected, fml);

            fml = &quot;=MAP({1,2,3},LAMBDA(x,SUM(x)))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 0, 2);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;1&quot;, &quot;2&quot;, &quot;3&quot; }, cells, expected, fml);

            fml = &quot;=MAP({1,2,3,4},{5,6,7,8},LAMBDA(x,y,SUM(x,y)))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 0, 3);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;6&quot;, &quot;8&quot;, &quot;10&quot;, &quot;12&quot; }, cells, expected, fml);

            fml = &quot;=MAP({1,2,3},{4,5,6},{-2,-3,-4},LAMBDA(x,y,z,SUM(x,y,z)))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 0, 2);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;3&quot;, &quot;4&quot;, &quot;5&quot; }, cells, expected, fml);

            fml = &quot;=SCAN(,B1:B5,LAMBDA(x,y,y+1))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 4, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;0&quot;, &quot;1&quot;, &quot;1&quot;, &quot;1&quot;, &quot;1&quot; }, cells, expected, fml);

            fml = &quot;=SCAN(,B1:B4,LAMBDA(x,y,x))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 3, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;0&quot;, &quot;0&quot;, &quot;0&quot;, &quot;0&quot; }, cells, expected, fml);

            fml = &quot;=SCAN(1,B1:B5,LAMBDA(x,y,x))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 4, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;1&quot;, &quot;1&quot;, &quot;1&quot;, &quot;1&quot;, &quot;1&quot; }, cells, expected, fml);

            fml = &quot;=SCAN(1,B1:B4,LAMBDA(x,y,x+y))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 3, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;1&quot;, &quot;1&quot;, &quot;1&quot;, &quot;1&quot; }, cells, expected, fml);

            fml = &quot;=SCAN(1,B1:B5,LAMBDA(x,y,x+y+1))&quot;;
            cell.SetDynamicArrayFormula(fml, new FormulaParseOptions(), true);
            expected = CellArea.CreateCellArea(0, 0, 4, 0);
            AssertHelper.checkCellArea(expected, cell.GetArrayRange(), fml + &quot;.ArrayRange&quot;);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, &quot;&quot;);
            DynamicFormulaTest.CheckResult(new string[] { &quot;2&quot;, &quot;3&quot;, &quot;4&quot;, &quot;5&quot;, &quot;6&quot; }, cells, expected, fml);
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



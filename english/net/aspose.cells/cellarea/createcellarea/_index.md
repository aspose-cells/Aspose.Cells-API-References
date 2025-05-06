---
title: CellArea.CreateCellArea
second_title: Aspose.Cells for .NET API Reference
description: CellArea method. Creates a cell area
type: docs
url: /net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column. |
| endRow | Int32 | The end row. |
| endColumn | Int32 | The end column. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: expected = CellArea.CreateCellArea(4, 0, 6, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Cells cells1 = wb.Worksheets[0].Cells;
            Cells cells2 = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            string fml1 = &quot;=FILTER(Sheet2!B2:B3,Sheet2!B2:B3&gt;1)&quot;;
            string fml2 = &quot;=FILTER(Sheet1!C1:C3,C1:C3&gt;1)&quot;;
            string fml3 = &quot;=FILTER(Sheet2!B5#,Sheet2!B5#&gt;1)&quot;;
            cells1[0, 0].SetDynamicArrayFormula(fml1, new FormulaParseOptions(), true);
            cells2[0, 1].SetDynamicArrayFormula(fml2, new FormulaParseOptions(), true);
            cells1[4, 0].SetDynamicArrayFormula(fml3, new FormulaParseOptions(), true);
            cells2[4, 1].SetDynamicArrayFormula(fml2, new FormulaParseOptions(), true);
            cells1[0, 2].PutValue(2);
            cells1[1, 2].PutValue(3);
            cells1[2, 2].PutValue(4);
            cells2[0, 2].PutValue(5);
            cells2[1, 2].PutValue(6);
            cells2[2, 2].PutValue(7);
            wb.RefreshDynamicArrayFormulas(true);
            CellArea expected = CellArea.CreateCellArea(0, 0, 1, 0);
            AssertHelper.checkCellArea(expected, cells1[0, 0].GetArrayRange(), &quot;Sheet1!A1.ArrayRange&quot;);
            CheckArrayFormula(fml1, cells1, expected, &quot;&quot;);
            CheckResult(new string[] { &quot;3&quot;, &quot;4&quot; }, cells1, expected, fml1);
            expected = CellArea.CreateCellArea(0, 1, 2, 1);
            AssertHelper.checkCellArea(expected, cells2[0, 1].GetArrayRange(), &quot;Sheet2!B1.ArrayRange&quot;);
            CheckArrayFormula(fml2, cells2, expected, &quot;&quot;);
            CheckResult(new string[] { &quot;2&quot;, &quot;3&quot;, &quot;4&quot; }, cells2, expected, fml2);

            expected = CellArea.CreateCellArea(4, 0, 6, 0);
            AssertHelper.checkCellArea(expected, cells1[4, 0].GetArrayRange(), &quot;Sheet1!A5.ArrayRange&quot;);
            CheckArrayFormula(fml3, cells1, expected, &quot;&quot;);
            CheckResult(new string[] { &quot;2&quot;, &quot;3&quot;, &quot;4&quot; }, cells1, expected, fml3);
            expected = CellArea.CreateCellArea(4, 1, 6, 1);
            AssertHelper.checkCellArea(expected, cells2[4, 1].GetArrayRange(), &quot;Sheet2!B5.ArrayRange&quot;);
            CheckArrayFormula(fml2, cells2, expected, &quot;&quot;);
            CheckResult(new string[] { &quot;2&quot;, &quot;3&quot;, &quot;4&quot; }, cells2, expected, fml2);
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Creates a cell area.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |

### Return Value

Return a [`CellArea`](../).

### Examples

```csharp
// Called: CellsNet57571(Constants.PivotTableSourcePath + &amp;quot;CELLSNET-57571.xlsx&amp;quot;, CellArea.CreateCellArea(&amp;quot;J15&amp;quot;, &amp;quot;N15&amp;quot;));
[Test]
        public void Method_String_()
        {
            Method_String_(Constants.PivotTableSourcePath + &quot;CellsNet57571.xlsx&quot;,CellArea.CreateCellArea(&quot;J15&quot;, &quot;O16&quot;));
            Method_String_(Constants.PivotTableSourcePath + &quot;CellsNet57571.xlsx&quot;, CellArea.CreateCellArea(&quot;J16&quot;, &quot;O16&quot;));
            Method_String_(Constants.PivotTableSourcePath + &quot;CellsNet57571.xlsx&quot;, CellArea.CreateCellArea(&quot;J15&quot;, &quot;N16&quot;));
            Method_String_(Constants.PivotTableSourcePath + &quot;CELLSNET-57571.xlsx&quot;, CellArea.CreateCellArea(&quot;J15&quot;, &quot;N15&quot;));
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



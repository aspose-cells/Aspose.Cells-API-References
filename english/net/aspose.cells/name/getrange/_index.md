---
title: Name.GetRange
second_title: Aspose.Cells for .NET API Reference
description: Name method. Gets the range if this name refers to a range
type: docs
url: /net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Gets the range if this name refers to a range.

```csharp
public Range GetRange()
```

### Return Value

The range.

### Examples

```csharp
// Called: Assert.IsNull(n.GetRange());
[Test]
        public void Method_GetRange()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;DefinedName/J43969.xlsx&quot;);
            Name n = wb.Worksheets.Names[0];
            Assert.IsNull(n.GetRange());
            FormulaCaseUtil.AssertInt(0, wb.Worksheets[0].CalculateFormula(&quot;=&quot; + n.Text,
                new CalculationOptions() { IgnoreError = false }), &quot;Calculate reference to the name&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Gets the range if this name refers to a range

```csharp
public Range GetRange(bool recalculate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | Boolean | whether recalculate it if this name has been calculated before this invocation. |

### Return Value

The range.

### Examples

```csharp
// Called: Aspose.Cells.Range r = name.GetRange(true);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 4; i++)
            {
                cells[i, 1].PutValue(i);
            }
            Name name = wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;testname&quot;)];
            string fml = &quot;IFERROR(Sheet1!$B$2:$B$4,-1)&quot;;
            name.RefersTo = fml;
            cells[&quot;C1&quot;].Formula = &quot;=testname&quot;;
            cells[&quot;D1&quot;].Formula = &quot;SUM(testname)&quot;;
            cells[&quot;E1&quot;].Formula = fml;
            cells[&quot;F1&quot;].Formula = &quot;SUM(&quot; + fml + &quot;)&quot;;
            wb.CalculateFormula(false);
            Assert.AreEqual(-1.0, cells[&quot;E1&quot;].DoubleValue, &quot;E1&quot;);
            Assert.AreEqual(-1.0, cells[&quot;F1&quot;].DoubleValue, &quot;E1&quot;);
            Assert.AreEqual(1.0, cells[&quot;C1&quot;].DoubleValue, &quot;C1&quot;);
            Assert.AreEqual(6.0, cells[&quot;D1&quot;].DoubleValue, &quot;D1&quot;);
            Aspose.Cells.Range r = name.GetRange(true);
            if (r == null || r.FirstRow != 1 || r.FirstColumn != 1 || r.RowCount != 3 || r.ColumnCount != 1)
            {
                Assert.Fail(&quot;Name.GetRange should return B2:B4&quot;);
            }
            Chart chart = wb.Worksheets[0].Charts[wb.Worksheets[0].Charts.Add(ChartType.Column, 10, 1, 20, 5)];
            chart.NSeries.Add(&quot;testname&quot;, true);
            Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, &quot;ChartDataCount&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The according sheet index. |
| row | Int32 | The according row index. |
| column | Int32 | The according column index |

### Return Value

The range.

### Examples

```csharp
// Called: Aspose.Cells.Range range = workbook.Worksheets.Names[&amp;quot;SubCat&amp;quot;].GetRange(0, 1, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42868.xlsx&quot;);
            Aspose.Cells.Range range = workbook.Worksheets.Names[&quot;SubCat&quot;].GetRange(0, 1, 1);
            Assert.AreEqual(&quot;=Defind!C2:C4&quot;, range.RefersTo.Replace(&quot;$&quot;, &quot;&quot;), &quot;Aspose.Cells.Range.RefersTo&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



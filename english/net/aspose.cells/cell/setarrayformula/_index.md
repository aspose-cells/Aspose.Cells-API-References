---
title: Cell.SetArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Sets an array formula to a range of cells
type: docs
url: /net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Sets an array formula to a range of cells.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| isR1C1 | Boolean | whether the formula is R1C1 formula |
| isLocal | Boolean | whether the formula is locale formatted |

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int) {#setarrayformula}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |

### Examples

```csharp
// Called: cells[&amp;quot;C2&amp;quot;].SetArrayFormula(&amp;quot;=FREQUENCY(A2:A10,B2:B4)&amp;quot;, 4, 1);
[Test, Category(&quot;Bug&quot;)]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_148783.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;C2&quot;].SetArrayFormula(&quot;=FREQUENCY(A2:A10,B2:B4)&quot;, 4, 1);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            workbook.CalculateFormula();

            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C2&quot;].DoubleValue ,1);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C3&quot;].DoubleValue, 2);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C4&quot;].DoubleValue, 4);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C5&quot;].DoubleValue, 2);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Sets an array formula to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |

### Examples

```csharp
// Called: cells[1, 0].SetArrayFormula(fmls[0], 2, 1, new FormulaParseOptions());
[Test]
        public void Method_FormulaParseOptions_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets.Add(&quot;Sheet2&quot;).Cells;
            cells[1, 0].SetArrayFormula(&quot;=TRANSPOSE(Sheet1!C1:E1)&quot;, 2, 1, new FormulaParseOptions());
            cells[1, 1].SetDynamicArrayFormula(&quot;=TRANSPOSE(Sheet1!C1:E1)&quot;, new FormulaParseOptions(), false);

            cells = wb.Worksheets[0].Cells;
            cells[0, 0].Formula = &quot;=B1&quot;;
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue(2);
            cells[0, 3].PutValue(4);
            cells[0, 4].PutValue(8);
            string[] fmls = new string[]
            {
                &quot;=TRANSPOSE(C1:E1)&quot;, &quot;=TRANSPOSE(C1:E1)&quot;,
                &quot;=B1#&quot;, &quot;=$A$3#&quot;, &quot;=INDIRECT(\&quot;A2:B2\&quot;)#&quot;,
                &quot;=SUM(A2#)&quot;, &quot;=$A$1#&quot;, &quot;=SUM(Sheet2!A2#)&quot;,
                &quot;=A2#&quot;, &quot;=INDIRECT(\&quot;A2:A2\&quot;)#&quot;, &quot;=Sheet2!A2#&quot;,
                &quot;=$B$2#&quot;, &quot;=Sheet2!A2#:Sheet2!B2#&quot;,
            };
            int[][] vals = new int[][]
            {
                new int[]{2, 4, }, new int[]{2, 4, 8, },
                null, null, null,
                new int[]{6, }, new int[]{1, }, new int[]{6, },
                new int[]{2, 4, }, new int[]{2, 4, }, new int[]{2, 4, },
                new int[]{2, 4, 8, }, new int[]{2, 4, 0, }, new int[]{2, 4, 8, },
            };
            cells[1, 0].SetArrayFormula(fmls[0], 2, 1, new FormulaParseOptions());
            wb.CalculateFormula();
            for (int i = 1; i &lt; fmls.Length; i++)
            {
                cells[1, i].SetDynamicArrayFormula(fmls[i], new FormulaParseOptions(), true);
            }

            for (int i = 0; i &lt; 2; i++)
            {
                if (i &gt; 0)
                {
                    wb = Util.ReSave(wb, SaveFormat.Xlsx);
                    cells = wb.Worksheets[0].Cells;
                }
                for (int j = 0; j &lt; fmls.Length; j++)
                {
                    int[] cv = vals[j];
                    int h = cv == null ? 1 : cv.Length;
                    for (int k = h; k &gt; 0; k--)
                    {
                        Assert.AreEqual(fmls[j], cells[k, j].Formula,
                            ((char)(&apos;A&apos; + j)) + &quot;&quot; + (k + 1) + &quot;.Formula&quot;);
                    }
                    for (int k = h; k &lt; 3; k++)
                    {
                        Assert.IsNull(cells.CheckCell(k + 1, j), fmls[j]
                            + &quot; should not be spilled to &quot; + ((char)(&apos;A&apos; + j)) + &quot;&quot; + (k + 2));
                    }
                }
                for (int k = 1; k &lt; 4; k++)
                {
                    Assert.AreEqual(fmls[fmls.Length - 1], cells[k, fmls.Length].Formula,
                        ((char)(&apos;A&apos; + fmls.Length)) + &quot;&quot; + (k + 1) + &quot;.Formula&quot;);
                }
                wb.CalculateFormula(false);
                for (int j = 0; j &lt; vals.Length; j++)
                {
                    int[] cv = vals[j];
                    if (cv == null)
                    {
                        Cell cell = cells[1, j];
                        Assert.AreEqual(&quot;#REF!&quot;, cell.Value,
                            cell.Name + &quot;.Value(Formula=&quot; + cell.Formula + &quot;)&quot;);
                        continue;
                    }
                    for (int k = 0; k &lt; cv.Length; k++)
                    {
                        Cell cell = cells[k + 1, j];
                        Assert.AreEqual(cv[k], cell.IntValue,
                            cell.Name + &quot;.Value(Formula=&quot; + cell.Formula + &quot;)&quot;);
                    }
                }
            }
        }
```

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Sets an array formula to a range of cells.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given array formula |

### See Also

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



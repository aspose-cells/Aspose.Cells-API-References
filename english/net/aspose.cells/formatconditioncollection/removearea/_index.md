---
title: FormatConditionCollection.RemoveArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Removes conditional formatted cell range by index
type: docs
url: /net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Removes conditional formatted cell range by index.

```csharp
public void RemoveArea(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the conditional formatted cell range to be removed. |

### Examples

```csharp
// Called: fcc.RemoveArea(1);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 18, 1048575, 16382));
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1048570, 17));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;
            Cells cells = sheet.Cells;
            Random r = new Random();
            int[] flags = new int[1000];
            for (int i = 0; i &lt; 128; i++)
            {
                for (int j = 0; j &lt; 16; j++)
                {
                    int v = r.Next(flags.Length);
                    int f = flags[v];
                    if (f == 0)
                    {
                        cells[i, j].PutValue(&quot;U&quot; + v);
                        flags[v] = ((i &lt;&lt; 4) | j) + 1;
                    }
                    else
                    {
                        cells[i, j].PutValue(&quot;D&quot; + v);
                        if (f &gt; 0)
                        {
                            f--;
                            cells[f &gt;&gt; 4, f &amp; 0x0F].PutValue(&quot;D&quot; + v);
                            flags[v] = -1;
                        }
                    }
                }
            }
            flags = null;
            VerifyJ43108(wb);
            fcc.RemoveArea(1);
            fcc.RemoveArea(0);
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 1048500, 16382));
            VerifyJ43108(wb);
            fcc.AddArea(CellArea.CreateCellArea(1048502, 0, 1048575, 16380));
            VerifyJ43108(wb);
            fcc.RemoveArea(1);
            fcc.RemoveArea(0);
            fcc.AddArea(CellArea.CreateCellArea(10, 5, 1048575, 16382));
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 9, 16382));
            fcc.AddArea(CellArea.CreateCellArea(10, 0, 1048575, 4));
            VerifyJ43108(wb);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Remove conditional formatting int the range.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The startRow of the range. |
| startColumn | Int32 | The startColumn of the range. |
| totalRows | Int32 | The number of rows of the range. |
| totalColumns | Int32 | The number of columns of the range. |

### Return Value

Returns TRUE, this FormatCondtionCollection should be removed.

### Examples

```csharp
// Called: fcc.RemoveArea(row, col, 1, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            string[] formulas = new string[]
            {
                &quot;=$C$8=$C$7&quot;, &quot;=$E$8=$E$7&quot;, &quot;=$F$8=$F$7&quot;, &quot;=$G$8=$G$7&quot;, &quot;=$C$7=$C$6&quot;, &quot;=$E$7=$E$6&quot;,
                &quot;=$F$7=$F$6&quot;, &quot;=$G$7=$G$6&quot;, &quot;=$B$7=$B$5&quot;, &quot;=$D$7=$D$6&quot;, &quot;=$D$8=$D$7&quot;
            };
            string[] initialCells = new string[]
            {
                &quot;C8&quot;, &quot;E8&quot;, &quot;F8&quot;, &quot;G8&quot;, &quot;C7&quot;, &quot;E7&quot;, &quot;F7&quot;, &quot;G7&quot;, &quot;B7&quot;, &quot;D7&quot;, &quot;D8&quot;
            };
            Random rand = new Random();
            TimePerformance monitor = new TimePerformance(30);
            monitor.StartPerfTest();
            for (int i = 0; i &lt; formulas.Length; i++)
            {
                int idx = cfc.Add();
                FormatConditionCollection fcc = cfc[idx];
                int row, col;
                CellsHelper.CellNameToIndex(initialCells[i], out row, out col);
                CellArea ca = CellArea.CreateCellArea(row, col, row, col);
                fcc.AddArea(ca);

                idx = fcc.AddCondition(FormatConditionType.Expression);
                FormatCondition fc = fcc[idx];
                fc.Formula1 = formulas[i];
                fc.Style.Font.Color = Color.FromArgb(0, 97, 0);
                Console.WriteLine(&quot;Processing condition: &quot; + fcc[0].Formula1);
                // create single cell areas for about 1000 cells
                for (int j = 0; j &lt; 1000; j++)
                {
                    row = rand.Next(20000);
                    col = rand.Next(26);
                    fcc.RemoveArea(row, col, 1, 1);
                    // Add the cell to the collection in order to apply conditional formatting
                    CellArea area = CellArea.CreateCellArea(row, col, row, col);
                    fcc.AddArea(area);
                }
            }
            monitor.FinishPerfTest(&quot;Repeatedly remove and add areas for 1000 times&quot;);
        }
```

### See Also

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: Cell.IsDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the cells formula is dynamic array formulatrue or legacy array formulafalse
type: docs
url: /net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Indicates whether the cell's formula is dynamic array formula(true) or legacy array formula(false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Examples

```csharp
// Called: else if (cellBase.IsDynamicArrayFormula &amp;amp;&amp;amp; !cellBase.IsArrayHeader)
public static bool Property_IsDynamicArrayFormula(Workbook excelCalc, Workbook excelBase, CellBaseComparator errBase,
            double delta, int outputLimit)
        {
            int totalCount = 0;
            int scn = Math.Min(excelCalc.Worksheets.Count, excelBase.Worksheets.Count);
            int detailCount = 0;
            bool noErrBase = errBase == null;
            for (int i = 0; i &lt; scn; i++)
            {
                Cells cellsCalc = excelCalc.Worksheets[i].Cells;
                IEnumerator enCalc = cellsCalc.GetEnumerator();
                if (!enCalc.MoveNext())
                {
                    continue;
                }
                string sheetName = excelCalc.Worksheets[i].Name;
                int curCount = 0;
                Cells cellsBase = excelBase.Worksheets[i].Cells;
                IEnumerator enBase = cellsBase.GetEnumerator();
                Cell cellCalc = (Cell)enCalc.Current;
                bool moveCalc = true;
                Cell cellBase;
                bool moveBase;
                if (enBase.MoveNext())
                {
                    moveBase = true;
                    cellBase = (Cell)enBase.Current;
                }
                else
                {
                    moveBase = false;
                    cellBase = null;
                }
                while (true)
                {
                    if (!moveBase || cellBase.Row &gt; cellCalc.Row
                        || cellBase.Row == cellCalc.Row &amp;&amp; cellBase.Column &gt; cellCalc.Column)
                    {
                        bool check = true;
                        if (cellCalc.IsDynamicArrayFormula &amp;&amp; !cellCalc.IsArrayHeader)
                        {
                            CellArea ca = cellCalc.GetArrayRange();
                            Cell header = cellsBase.CheckCell(ca.StartRow, ca.StartColumn);
                            if (header != null &amp;&amp; header.IsDynamicArrayFormula
                                &amp;&amp; (noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column, null)))
                            {
                                check = false;
                                detailCount++;
                                if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                                {
                                    Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellCalc.Name
                                        + &quot;: extra dynamic array formula(may be incorrectly spilled range)&quot;);
                                }
                            }
                        }
                        if (check &amp;&amp; cellCalc.IsFormula &amp;&amp; (cellCalc.IsNumericValue || cellCalc.StringValue != &quot;&quot;)
                            &amp;&amp; (noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column, null)))
                        {
                            detailCount++;
                            if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                            {
                                Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellCalc.Name
                                    + &quot;: [null]-&gt;[&quot; + cellCalc.StringValue + &quot;]&quot;);
                            }
                        }
                        if (!enCalc.MoveNext())
                        {
                            break;
                        }
                        cellCalc = (Cell)enCalc.Current;
                        continue;
                    }
                    if (!moveCalc || cellBase.Row &lt; cellCalc.Row
                        || cellBase.Row == cellCalc.Row &amp;&amp; cellBase.Column &lt; cellCalc.Column)
                    {
                        if (cellBase.IsDynamicArrayFormula &amp;&amp; !cellBase.IsArrayHeader)
                        {
                            CellArea ca = cellBase.GetArrayRange();
                            Cell header = cellsCalc.CheckCell(ca.StartRow, ca.StartColumn);
                            if (header != null &amp;&amp; header.IsDynamicArrayFormula
                                &amp;&amp; (noErrBase || errBase.PutCell(sheetName, cellBase.Row, (short)cellBase.Column, null)))
                            {
                                detailCount++;
                                if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                                {
                                    Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellBase.Name
                                        + &quot;: absent dynamic array formula(may be incorrectly spilled range)&quot;);
                                }
                            }
                        }
                        if (!enBase.MoveNext())
                        {
                            break;
                        }
                        cellBase = (Cell)enBase.Current;
                        continue;
                    }
                    if (cellCalc.IsFormula)
                    {
                        curCount++;
                        bool check = true;
                        if (!cellBase.IsFormula &amp;&amp; cellCalc.IsDynamicArrayFormula &amp;&amp; !cellCalc.IsArrayHeader)
                        {
                            CellArea ca = cellCalc.GetArrayRange();
                            Cell header = cellsBase.CheckCell(ca.StartRow, ca.StartColumn);
                            if (header != null &amp;&amp; header.IsDynamicArrayFormula
                                &amp;&amp; (noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column, null)))
                            {
                                check = false;
                                detailCount++;
                                if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                                {
                                    Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellCalc.Name
                                        + &quot;: extra dynamic array formula(may be incorrectly spilled range)&quot;);
                                }
                            }
                        }
                        if (check &amp;&amp; !IsEqualValue(cellCalc, cellBase, delta))
                        {
                            string fml = cellCalc.Formula;
                            if (fml != null &amp;&amp; VolatileFunc.IsMatch(fml))
                            {
                                if (outputLimit &gt;= 0)
                                {
                                    Console.WriteLine(&quot;Ignore volatile function for [&quot; + i + &quot;]&quot;
                                        + sheetName + &quot;!&quot; + cellCalc.Name + &quot;: &quot; + fml);
                                }
                            }
                            else if (cellCalc.IsNumericValue &amp;&amp; cellBase.IsNumericValue)
                            {
                                if ((noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column,
                                    BitConverter.GetBytes(cellCalc.DoubleValue - cellBase.DoubleValue))))
                                {
                                    detailCount++;
                                    if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                                    {
                                        Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellCalc.Name
                                           + &quot;: [&quot; + cellBase.DoubleValue + &quot;]-&gt;[&quot; + cellCalc.DoubleValue + &quot;]&quot;);
                                    }
                                }
                            }
                            else if ((noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column, null)))
                            {
                                detailCount++;
                                if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                                {
                                    Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellCalc.Name
                                        + &quot;: [&quot; + cellBase.Value + &quot;]-&gt;[&quot; + cellCalc.Value + &quot;]&quot;);
                                }
                            }
                        }
                    }
                    else if (cellBase.IsDynamicArrayFormula &amp;&amp; !cellBase.IsArrayHeader)
                    {
                        CellArea ca = cellBase.GetArrayRange();
                        Cell header = cellsCalc.CheckCell(ca.StartRow, ca.StartColumn);
                        if (header != null &amp;&amp; header.IsDynamicArrayFormula
                            &amp;&amp; (noErrBase || errBase.PutCell(sheetName, cellCalc.Row, (short)cellCalc.Column, null)))
                        {
                            detailCount++;
                            if (outputLimit &lt; 0 &amp;&amp; detailCount &lt; -outputLimit || detailCount &lt; outputLimit)
                            {
                                Console.WriteLine(&quot;[&quot; + i + &quot;]&quot; + sheetName + &quot;!&quot; + cellBase.Name
                                    + &quot;: absent dynamic array formula(may be incorrectly spilled range)&quot;);
                            }
                        }
                    }
                    if (enCalc.MoveNext())
                    {
                        cellCalc = (Cell)enCalc.Current;
                    }
                    else if (!moveBase)
                    {
                        break;
                    }
                    else
                    {
                        moveCalc = false;
                    }
                    if (enBase.MoveNext())
                    {
                        cellBase = (Cell)enBase.Current;
                    }
                    else if (!moveCalc)
                    {
                        break;
                    }
                    else
                    {
                        moveBase = false;
                    }
                }
                //Console.WriteLine(sheetName + &quot;: formula count is &quot; + curCount);
                totalCount += curCount;
            }
            Console.WriteLine(&quot;Total formula count in workbook is &quot; + totalCount + &quot;; Error count is &quot; + detailCount);
            if (noErrBase &amp;&amp; detailCount &gt; 0)
            {
                Console.WriteLine(&quot;xxxxxxxxxxxxxxxxxxxxxxxxxEXTRA ERROR BEGINxxxxxxxxxxxxxxxxxxxxxxxxx&quot;);
                Console.WriteLine(&quot;There is no error base, so ALL errors are EXTRA ERROR.&quot;);
                Console.WriteLine(&quot;xxxxxxxxxxxxxxxxxxxxxxxxxxEXTRA ERROR ENDxxxxxxxxxxxxxxxxxxxxxxxxxx&quot;);
            }
            if (detailCount &gt; Math.Abs(outputLimit))
            {
                Console.WriteLine(&quot;There are &quot; + (detailCount - outputLimit) + &quot; more errors have not been shown here.&quot;);
                return true;
            }
            return detailCount &lt; 1;
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



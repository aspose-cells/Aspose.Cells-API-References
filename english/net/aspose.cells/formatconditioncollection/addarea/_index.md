---
title: FormatConditionCollection.AddArea
second_title: Aspose.Cells for .NET API Reference
description: FormatConditionCollection method. Adds a conditional formatted cell range
type: docs
url: /net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Adds a conditional formatted cell range.

```csharp
public int AddArea(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | Conditional formatted cell range. |

### Return Value

Conditional formatted cell rang index.

### Examples

```csharp
// Called: fcc.AddArea(CellArea.CreateCellArea(2, 0, 7, 0));
[Test]
        public void Method_CellArea_()
        {
            Workbook wb = new Workbook();
            int v0 = wb.DefaultStyle.Font.Size;
            int v1 = v0 + 5;
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 10; i++)
            {
                for (int j = 0; j &lt; 7; j++)
                {
                    cells[i, j].PutValue(i + 1);
                }
            }
            string[] fmls = new string[] { &quot;=SUM(D2:E3)&gt;F1&quot; };
            ConditionalFormattingCollection cfc = wb.Worksheets[0].ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(2, 0, 7, 0));
            fcc.AddArea(CellArea.CreateCellArea(2, 2, 7, 2));
            FormatCondition fc = fcc[fcc.AddCondition(FormatConditionType.Expression)];
            fc.Formula1 = fmls[0];
            fc.Style.Font.Size = v1;
            for (int i = 1; i &lt; 9; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    bool applied = (j == 0 || j == 2) &amp;&amp; i &gt; 1 &amp;&amp; i &lt; 8;
                    CheckCellFormatConditions(cells[i, j], applied ? v1 : v0, applied ? fmls : null,
                        &quot;With original conditional formatting,&quot;);
                }
            }
            cells.InsertRange(CellArea.CreateCellArea(2, 3, 4, 4), ShiftType.Down);
            CheckEmptyAppliedRange(cfc, &quot;After inserting range,&quot;);
            fmls[0] = &quot;=SUM(D2:E6)&gt;F1&quot;;
            string[] fmls1 = new string[] { &quot;=SUM(F2:G3)&gt;H1&quot; };
            string[] fmls2 = new string[] { &quot;=SUM(D6:E7)&gt;F2&quot; };
            for (int i = 1; i &lt; 9; i++)
            {
                for (int j = 0; j &lt; 4; j++)
                {
                    bool applied = (j == 0 || j == 2) &amp;&amp; i &gt; 1 &amp;&amp; i &lt; 8;
                    CheckCellFormatConditions(cells[i, j], applied ? v1 : v0,
                        applied ? (j == 2 ? fmls1 : (i &gt; 2 ? fmls2 : fmls)) : null,
                        &quot;After inserting range,&quot;);
                }
            }
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



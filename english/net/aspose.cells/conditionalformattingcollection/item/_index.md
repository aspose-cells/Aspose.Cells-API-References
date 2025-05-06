---
title: ConditionalFormattingCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection property. Gets the FormatConditions element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingcollection/item/
---
## ConditionalFormattingCollection indexer

Gets the FormatConditions element at the specified index.

```csharp
public FormatConditionCollection this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Examples

```csharp
// Called: FormatConditionCollection fConditions = cformattings[i];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings\\ConditionalFormattings2.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;            
            CellArea cellarea;
            FormatCondition fCondition;
            for (int i = 0; i &lt; cformattings.Count; i++)
            {
                FormatConditionCollection fConditions = cformattings[i];
                for (int j = 0; j &lt; fConditions.RangeCount; j++)
                {
                    cellarea = fConditions.GetCellArea(j);
                    if ((cellarea.StartRow == 1 &amp;&amp; cellarea.EndRow == 1 &amp;&amp; cellarea.StartColumn == 2 &amp;&amp; cellarea.EndColumn == 2) ||
                        (cellarea.StartRow == 3 &amp;&amp; cellarea.EndRow == 3 &amp;&amp; cellarea.StartColumn == 2 &amp;&amp; cellarea.EndColumn == 2) ||
                        (cellarea.StartRow == 6 &amp;&amp; cellarea.EndRow == 6 &amp;&amp; cellarea.StartColumn == 2 &amp;&amp; cellarea.EndColumn == 2) ||
                        (cellarea.StartRow ==5 &amp;&amp; cellarea.EndRow==5 &amp;&amp; cellarea.StartColumn==5 &amp;&amp; cellarea.EndColumn ==5) ||
                        (cellarea.StartRow == 7 &amp;&amp; cellarea.EndRow == 7 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp; cellarea.EndColumn == 5) ||
                        (cellarea.StartRow == 9 &amp;&amp; cellarea.EndRow == 9 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp; cellarea.EndColumn == 5) ||
                        (cellarea.StartRow == 11 &amp;&amp; cellarea.EndRow == 11 &amp;&amp; cellarea.StartColumn == 5 &amp;&amp; cellarea.EndColumn == 5))
                    {
                        continue;
                    }
                    AssertHelper.Fail(&quot;fail&quot;);
                }
                for (int k = 0; k &lt; fConditions.Count; k++)
                {
                    fCondition = fConditions[k];
                    check(fCondition);
                }
            }
        }
```

### See Also

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



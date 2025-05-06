---
title: FormatCondition.Priority
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values where 1 is the highest priority
type: docs
url: /net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

```csharp
public int Priority { get; set; }
```

### Examples

```csharp
// Called: int p = fcc[i].Priority;
[Test]
        public void Property_Priority()
        {
            Workbook src = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/N49693.xlsx&quot;);
            Workbook dest = new Workbook();
            Worksheet destSheet = dest.Worksheets[0];
            Aspose.Cells.Range sourceRange = src.Worksheets[0].Cells.MaxDisplayRange;
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange(sourceRange.FirstRow,
                               sourceRange.FirstColumn,
                               sourceRange.RowCount, sourceRange.ColumnCount);
            destRange.Copy(sourceRange);
            int totalRowCount = sourceRange.RowCount;
            sourceRange = src.Worksheets[1].Cells.MaxDisplayRange;
            destRange = destSheet.Cells.CreateRange(sourceRange.FirstRow + totalRowCount,
                               sourceRange.FirstColumn,
                               sourceRange.RowCount, sourceRange.ColumnCount);
            destRange.Copy(sourceRange);
            ConditionalFormattingCollection cfc = destSheet.ConditionalFormattings;
            Hashtable ps = new Hashtable();
            object v = true;
            foreach(FormatConditionCollection fcc in cfc)
            {
                for(int i=fcc.Count-1; i&gt;-1; i--)
                {
                    int p = fcc[i].Priority;
                    if(ps.ContainsKey(p))
                    {
                        Assert.Fail(&quot;Duplicated priority value: &quot; + p);
                    }
                    ps.Add(p, v);
                }
            }
            Util.SaveManCheck(dest, &quot;ConditionalFormattings&quot;, &quot;N49693_res.xlsx&quot;);
        }
```

### See Also

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



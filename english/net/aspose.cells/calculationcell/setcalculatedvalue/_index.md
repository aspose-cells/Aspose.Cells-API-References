---
title: CalculationCell.SetCalculatedValue
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell method. Sets the calculated value for the cell
type: docs
url: /net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Sets the calculated value for the cell.

```csharp
public void SetCalculatedValue(object v)
```

### Remarks

User can set the calculated result by this method to ignore the automatic calculation for the cell.

### Examples

```csharp
// Called: cc.SetCalculatedValue(101);
public override bool Method_Object_(IEnumerator circularCellsData)
            {
                CalculationCell cc = null;
                StringBuilder sb = new StringBuilder();
                int sheetIndex = -1;
                while (circularCellsData.MoveNext())
                {
                    cc = (CalculationCell)circularCellsData.Current;
                    sb.Append(&quot;-&gt;&quot;);
                    if (sheetIndex != cc.Worksheet.Index)
                    {
                        sb.Append(cc.Worksheet.Name).Append(&apos;!&apos;);
                        sheetIndex = cc.Worksheet.Index;
                    }
                    sb.Append(CellsHelper.CellIndexToName(cc.CellRow, cc.CellColumn));
                    if (mFlag == 1)
                    {
                        if (cc.CellRow % 2 == 0)
                        {
                            cc.SetCalculatedValue(111);
                        }
                    }
                    else if (mFlag == 3 &amp;&amp; cc.CellRow % 2 == 1)
                    {
                        cc.SetCalculatedValue(101);
                    }
                }
                Assert.AreEqual(mCirculars[mCount], sb.ToString(2, sb.Length - 2), &quot;Circle[&quot; + mCount + &quot;] for flag &quot; + mFlag);
                mCount++;
                return (mFlag &amp; 0x02) != 0;
            }
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



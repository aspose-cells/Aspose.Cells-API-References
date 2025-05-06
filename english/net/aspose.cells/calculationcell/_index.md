---
title: Class CalculationCell
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CalculationCell class. Represents the calculation relevant data about one cell which is being calculated
type: docs
url: /net/aspose.cells/calculationcell/
---
## CalculationCell class

Represents the calculation relevant data about one cell which is being calculated.

```csharp
public class CalculationCell
```

## Properties

| Name | Description |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Gets the Cell object which is being calculated. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Gets the column index of the cell. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Gets the row index of the cell. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Gets the Workbook object. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Gets the Worksheet object where the cell is in. |

## Methods

| Name | Description |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Sets the calculated value for the cell. |

### Remarks

All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

### Examples

```csharp
// Called: CalculationCell cc = null;
public override bool Type_CalculationCell(IEnumerator circularCellsData)
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



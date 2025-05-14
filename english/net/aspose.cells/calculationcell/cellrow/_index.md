---
title: CalculationCell.CellRow
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the row index of the cell
type: docs
url: /net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Gets the row index of the cell.

```csharp
public int CellRow { get; }
```

### Examples

```csharp
// Called: else if (mFlag == 3 && cc.CellRow % 2 == 1)
public override bool CalculationCell_Property_CellRow(IEnumerator circularCellsData)
            {
                CalculationCell cc = null;
                StringBuilder sb = new StringBuilder();
                int sheetIndex = -1;
                while (circularCellsData.MoveNext())
                {
                    cc = (CalculationCell)circularCellsData.Current;
                    sb.Append("->");
                    if (sheetIndex != cc.Worksheet.Index)
                    {
                        sb.Append(cc.Worksheet.Name).Append('!');
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
                    else if (mFlag == 3 && cc.CellRow % 2 == 1)
                    {
                        cc.SetCalculatedValue(101);
                    }
                }
                Assert.AreEqual(mCirculars[mCount], sb.ToString(2, sb.Length - 2), "Circle[" + mCount + "] for flag " + mFlag);
                mCount++;
                return (mFlag & 0x02) != 0;
            }
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



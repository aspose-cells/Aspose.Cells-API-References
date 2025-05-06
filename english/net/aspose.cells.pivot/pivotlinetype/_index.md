---
title: Enum PivotLineType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotLineType enum. Specifies the type of the PivotLine
type: docs
url: /net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Specifies the type of the PivotLine.

```csharp
public enum PivotLineType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Regular | `0` | Regular PivotLine with pivot items. |
| Subtotal | `1` | Subtotal line. |
| GrandTotal | `2` | Grand Total line. |
| Blank | `3` | Blank line after each group. |

### Examples

```csharp
// Called: workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &amp;quot;K15&amp;quot;);
[Test]
        public void Type_PivotLineType()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET46200_1.xlsx&quot;);
            workbook.Worksheets[0].PivotTables[0].RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, &quot;K15&quot;);
            workbook.Worksheets[0].PivotTables[0].CalculateData();
            Assert.AreEqual(&quot;1&quot;, workbook.Worksheets[0].Cells[&quot;K17&quot;].StringValue);
        
        }
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



---
title: PivotField.Number
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the builtin display format of numbers and dates
type: docs
url: /net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Represents the built-in display format of numbers and dates.

```csharp
public int Number { get; set; }
```

### Examples

```csharp
// Called: pivotField.Number = 14;
private void Property_Number(PivotTable pivotTable, string fieldName, string caption,
            bool subTotals = false,
            bool layoutInOutline = false,
            bool layoutBlankLine = false,
            bool layoutCompactRow = false,
            bool layoutSubtotalAtTop = false,
            string numberFormat = &quot;&quot;,
            bool hideDetail = false,
            bool isAutoSort = false,
            bool isDate = false)
        {
            PivotField pivotField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, fieldName)];
            pivotField.DisplayName = caption;
            pivotField.ShowCompact = layoutCompactRow;
            pivotField.ShowInOutlineForm = layoutInOutline;
            pivotField.ShowSubtotalAtTop = layoutSubtotalAtTop;
            pivotField.InsertBlankRow = layoutBlankLine;
            pivotField.IsAutoSubtotals = subTotals;
            pivotField.NumberFormat = numberFormat;
            pivotField.HideDetail(hideDetail);
            pivotField.IsAutoSort = isAutoSort;
            if (isDate)
            {
                pivotField.Number = 14;
            }
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



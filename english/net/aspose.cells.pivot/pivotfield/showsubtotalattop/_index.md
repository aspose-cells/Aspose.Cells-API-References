---
title: PivotField.ShowSubtotalAtTop
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. when ShowInOutlineForm is true then display subtotals at the top of the list of items instead of at the bottom
type: docs
url: /net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Remarks

Only works when ShowInOutlineForm is true.

### Examples

```csharp
// Called: pivotField.ShowSubtotalAtTop = layoutSubtotalAtTop;
private void PivotField_Property_ShowSubtotalAtTop(PivotTable pivotTable, string fieldName, string caption,
            bool subTotals = false,
            bool layoutInOutline = false,
            bool layoutBlankLine = false,
            bool layoutCompactRow = false,
            bool layoutSubtotalAtTop = false,
            string numberFormat = "",
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



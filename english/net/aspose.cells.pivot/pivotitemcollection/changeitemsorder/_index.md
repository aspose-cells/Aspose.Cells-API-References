---
title: PivotItemCollection.ChangeitemsOrder
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection method. Directly changes the orders of the two items
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Directly changes the orders of the two items.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotItemCollection.SwapItem() method. This method will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: items.ChangeitemsOrder(1, 2);
[Test]
        public void Method_Int32_()
        {
            var wb = new Workbook(Constants.openPivottablePath + &quot;rrr.xlsx&quot;);
            Aspose.Cells.Pivot.PivotTable pivotTable = wb.Worksheets[0].PivotTables[0];
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            items[0].Move(1,false);
            items.ChangeitemsOrder(2, 3);
            items.ChangeitemsOrder(1, 2);
            wb.Save(Constants.savePivottablePath + &quot;29480.xlsx&quot;);

        }
```

### See Also

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



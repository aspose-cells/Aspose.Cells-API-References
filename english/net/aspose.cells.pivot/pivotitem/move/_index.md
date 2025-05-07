---
title: PivotItem.Move
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Moves the item up or down
type: docs
url: /net/aspose.cells.pivot/pivotitem/move/
---
## PivotItem.Move method

Moves the item up or down

```csharp
public void Move(int count, bool isSameParent)
```

| Parameter | Type | Description |
| --- | --- | --- |
| count | Int32 | The number of moving up or down. Move the item up if this is less than zero; Move the item down if this is greater than zero. |
| isSameParent | Boolean | Specifying whether moving operation is in the same parent node or not |

### Examples

```csharp
// Called: items[0].Move(1,false);
[Test]
        public void Method_Boolean_()
        {
            var wb = new Workbook(Constants.openPivottablePath + "rrr.xlsx");
            Aspose.Cells.Pivot.PivotTable pivotTable = wb.Worksheets[0].PivotTables[0];
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            items[0].Move(1,false);
            items.ChangeitemsOrder(2, 3);
            items.ChangeitemsOrder(1, 2);
            wb.Save(Constants.savePivottablePath + "29480.xlsx");

        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



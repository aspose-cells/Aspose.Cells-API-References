---
title: PivotField.DragToRow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field can be dragged to the row position. The default value is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/dragtorow/
---
## PivotField.DragToRow property

Indicates whether the specified field can be dragged to the row position. The default value is true.

```csharp
public bool DragToRow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(pfieldSrc.DragToRow, pfieldDest.DragToRow, info + &amp;quot;.DragToRow&amp;quot;);
public static void Property_DragToRow(PivotField pfieldSrc, PivotField pfieldDest, string info)
        {
            if (AssertHelper.checkNull(pfieldSrc, pfieldDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(pfieldSrc.AutoShowCount, pfieldDest.AutoShowCount, info + &quot;.AutoShowCount&quot;);
            AssertHelper.AreEqual(pfieldSrc.AutoShowField, pfieldDest.AutoShowField, info + &quot;.AutoShowField&quot;);
            AssertHelper.AreEqual(pfieldSrc.AutoSortField, pfieldDest.AutoSortField, info + &quot;.AutoSortField&quot;);
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseFieldIndex, pfieldDest.ShowValuesSetting.BaseFieldIndex, info + &quot;.BaseField&quot;);
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseItemIndex, pfieldDest.ShowValuesSetting.BaseItemIndex, info + &quot;.BaseItem&quot;);
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseItemPositionType, pfieldDest.ShowValuesSetting.BaseItemPositionType, info + &quot;.BaseItemPosition&quot;);
            AssertHelper.AreEqual(pfieldSrc.CurrentPageItem, pfieldDest.CurrentPageItem, info + &quot;.CurrentPageItem&quot;);
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.CalculationType, pfieldDest.ShowValuesSetting.CalculationType, info + &quot;.DataDisplayFormat&quot;);
            AssertHelper.AreEqual(pfieldSrc.DisplayName, pfieldDest.DisplayName, info + &quot;.DisplayName&quot;);
            AssertHelper.AreEqual(pfieldSrc.DragToColumn, pfieldDest.DragToColumn, info + &quot;.DragToColumn&quot;);
            AssertHelper.AreEqual(pfieldSrc.DragToHide, pfieldDest.DragToHide, info + &quot;.DragToHide&quot;);
            AssertHelper.AreEqual(pfieldSrc.DragToPage, pfieldDest.DragToPage, info + &quot;.DragToPage&quot;);
            AssertHelper.AreEqual(pfieldSrc.DragToRow, pfieldDest.DragToRow, info + &quot;.DragToRow&quot;);
            AssertHelper.AreEqual(pfieldSrc.Function, pfieldDest.Function, info + &quot;.Function&quot;);
            //AssertHelper.AreEqual(pfieldSrc.GetSubtotals
            AssertHelper.AreEqual(pfieldSrc.IsAscendShow, pfieldDest.IsAscendShow, info + &quot;.IsAscendShow&quot;);
            AssertHelper.AreEqual(pfieldSrc.IsAscendSort, pfieldDest.IsAscendSort, info + &quot;.IsAscendSort&quot;);
            AssertHelper.AreEqual(pfieldSrc.IsAutoShow, pfieldDest.IsAutoShow, info + &quot;.IsAutoShow&quot;);
            AssertHelper.AreEqual(pfieldSrc.IsAutoSort, pfieldDest.IsAutoSort, info + &quot;.IsAutoSort&quot;);
            AssertHelper.AreEqual(pfieldSrc.IsAutoSubtotals, pfieldDest.IsAutoSubtotals, info + &quot;.IsAutoSubtotals&quot;);
            //AssertHelper.AreEqual(pfieldSrc.IsHiddenItem
            AssertHelper.AreEqual(pfieldSrc.Name, pfieldDest.Name, info + &quot;.Name&quot;);
            AssertHelper.AreEqual(pfieldSrc.Number, pfieldDest.Number, info + &quot;.Number&quot;);
            AssertHelper.AreEqual(pfieldSrc.NumberFormat, pfieldDest.NumberFormat, info + &quot;.NumberFormat&quot;);
            AssertHelper.AreEqual(pfieldSrc.Position, pfieldDest.Position, info + &quot;.Position&quot;);
            AssertHelper.AreEqual(pfieldSrc.ShowAllItems, pfieldDest.ShowAllItems, info + &quot;.ShowAllItems&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



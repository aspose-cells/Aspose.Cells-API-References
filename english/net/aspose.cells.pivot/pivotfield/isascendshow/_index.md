---
title: PivotField.IsAscendShow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is autoshown ascending
type: docs
url: /net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

Indicates whether the specified PivotTable field is autoshown ascending.

```csharp
public bool IsAscendShow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(pfieldSrc.IsAscendShow, pfieldDest.IsAscendShow, info + ".IsAscendShow");
public static void PivotField_Property_IsAscendShow(PivotField pfieldSrc, PivotField pfieldDest, string info)
        {
            if (AssertHelper.checkNull(pfieldSrc, pfieldDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(pfieldSrc.AutoShowCount, pfieldDest.AutoShowCount, info + ".AutoShowCount");
            AssertHelper.AreEqual(pfieldSrc.AutoShowField, pfieldDest.AutoShowField, info + ".AutoShowField");
            AssertHelper.AreEqual(pfieldSrc.AutoSortField, pfieldDest.AutoSortField, info + ".AutoSortField");
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseFieldIndex, pfieldDest.ShowValuesSetting.BaseFieldIndex, info + ".BaseField");
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseItemIndex, pfieldDest.ShowValuesSetting.BaseItemIndex, info + ".BaseItem");
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.BaseItemPositionType, pfieldDest.ShowValuesSetting.BaseItemPositionType, info + ".BaseItemPosition");
            AssertHelper.AreEqual(pfieldSrc.CurrentPageItem, pfieldDest.CurrentPageItem, info + ".CurrentPageItem");
            AssertHelper.AreEqual(pfieldSrc.ShowValuesSetting.CalculationType, pfieldDest.ShowValuesSetting.CalculationType, info + ".DataDisplayFormat");
            AssertHelper.AreEqual(pfieldSrc.DisplayName, pfieldDest.DisplayName, info + ".DisplayName");
            AssertHelper.AreEqual(pfieldSrc.DragToColumn, pfieldDest.DragToColumn, info + ".DragToColumn");
            AssertHelper.AreEqual(pfieldSrc.DragToHide, pfieldDest.DragToHide, info + ".DragToHide");
            AssertHelper.AreEqual(pfieldSrc.DragToPage, pfieldDest.DragToPage, info + ".DragToPage");
            AssertHelper.AreEqual(pfieldSrc.DragToRow, pfieldDest.DragToRow, info + ".DragToRow");
            AssertHelper.AreEqual(pfieldSrc.Function, pfieldDest.Function, info + ".Function");
            //AssertHelper.AreEqual(pfieldSrc.GetSubtotals
            AssertHelper.AreEqual(pfieldSrc.IsAscendShow, pfieldDest.IsAscendShow, info + ".IsAscendShow");
            AssertHelper.AreEqual(pfieldSrc.IsAscendSort, pfieldDest.IsAscendSort, info + ".IsAscendSort");
            AssertHelper.AreEqual(pfieldSrc.IsAutoShow, pfieldDest.IsAutoShow, info + ".IsAutoShow");
            AssertHelper.AreEqual(pfieldSrc.IsAutoSort, pfieldDest.IsAutoSort, info + ".IsAutoSort");
            AssertHelper.AreEqual(pfieldSrc.IsAutoSubtotals, pfieldDest.IsAutoSubtotals, info + ".IsAutoSubtotals");
            //AssertHelper.AreEqual(pfieldSrc.IsHiddenItem
            AssertHelper.AreEqual(pfieldSrc.Name, pfieldDest.Name, info + ".Name");
            AssertHelper.AreEqual(pfieldSrc.Number, pfieldDest.Number, info + ".Number");
            AssertHelper.AreEqual(pfieldSrc.NumberFormat, pfieldDest.NumberFormat, info + ".NumberFormat");
            AssertHelper.AreEqual(pfieldSrc.Position, pfieldDest.Position, info + ".Position");
            AssertHelper.AreEqual(pfieldSrc.ShowAllItems, pfieldDest.ShowAllItems, info + ".ShowAllItems");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



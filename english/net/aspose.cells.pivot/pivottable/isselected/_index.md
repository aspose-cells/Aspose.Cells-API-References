---
title: PivotTable.IsSelected
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether this PivotTable is selected
type: docs
url: /net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Indicates whether this PivotTable is selected.

```csharp
public bool IsSelected { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ptableSrc.IsSelected, ptableDest.IsSelected, info + &amp;quot;.IsSelected&amp;quot;);
public static void Property_IsSelected(PivotTable ptableSrc, PivotTable ptableDest, string info)
        {
            if (AssertHelper.checkNull(ptableSrc, ptableDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(ptableSrc.AutoFormatType, ptableDest.AutoFormatType, info + &quot;.AutoFormatType&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.BaseFields, ptableDest.BaseFields, info + &quot;.BaseFields&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.ColumnFields, ptableDest.ColumnFields, info + &quot;.ColumnFields&quot;);
            AssertHelper.AreEqual(ptableSrc.ShowColumnGrandTotals, ptableDest.ShowColumnGrandTotals, info + &quot;.ColumnGrand&quot;);
            CellAreaTest.Property_IsSelected(ptableSrc.ColumnRange, ptableDest.ColumnRange, info + &quot;.ColumnRange&quot;);
            CellAreaTest.Property_IsSelected(ptableSrc.DataBodyRange, ptableDest.DataBodyRange, info + &quot;.DataBordyRange&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.DataField, ptableDest.DataField, info + &quot;.DataField&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.DataFields, ptableDest.DataFields, info + &quot;.DataFields&quot;);
            AssertHelper.AreEqual(ptableSrc.DisplayErrorString, ptableDest.DisplayErrorString, info + &quot;.DisplayErrorString&quot;);
            AssertHelper.AreEqual(ptableSrc.DisplayImmediateItems, ptableDest.DisplayImmediateItems, info + &quot;.DisplayImmediateItems&quot;);
            AssertHelper.AreEqual(ptableSrc.DisplayNullString, ptableDest.DisplayNullString, info + &quot;.DisplayNullString&quot;);
            AssertHelper.AreEqual(ptableSrc.EnableDrilldown, ptableDest.EnableDrilldown, info + &quot;.EnableDrilldown&quot;);
            AssertHelper.AreEqual(ptableSrc.EnableFieldDialog, ptableDest.EnableFieldDialog, info + &quot;.EnableFieldDialog&quot;);
            AssertHelper.AreEqual(ptableSrc.EnableFieldList, ptableDest.EnableFieldList, info + &quot;.EnableFieldList&quot;);
            AssertHelper.AreEqual(ptableSrc.EnableWizard, ptableDest.EnableWizard, info + &quot;.EnableWizard&quot;);
            AssertHelper.AreEqual(ptableSrc.ErrorString, ptableDest.ErrorString, info + &quot;.ErrorString&quot;);
            AssertHelper.AreEqual(ptableSrc.IsAutoFormat, ptableDest.IsAutoFormat, info + &quot;.IsAutoFormat&quot;);
            AssertHelper.AreEqual(ptableSrc.IsSelected, ptableDest.IsSelected, info + &quot;.IsSelected&quot;);
            AssertHelper.AreEqual(ptableSrc.ManualUpdate, ptableDest.ManualUpdate, info + &quot;.ManualUpdate&quot;);
            AssertHelper.AreEqual(ptableSrc.MergeLabels, ptableDest.MergeLabels, info + &quot;.MergeLabels&quot;);
            AssertHelper.AreEqual(ptableSrc.Name, ptableDest.Name, info + &quot;.Name&quot;);
            AssertHelper.AreEqual(ptableSrc.NullString, ptableDest.NullString, info + &quot;.NullString&quot;);
            AssertHelper.AreEqual(ptableSrc.PageFieldOrder, ptableDest.PageFieldOrder, info + &quot;.PageFieldOrder&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.PageFields, ptableDest.PageFields, info + &quot;.PageFields&quot;);
            AssertHelper.AreEqual(ptableSrc.PageFieldWrapCount, ptableDest.PageFieldWrapCount, info + &quot;.PageFieldWrapCount&quot;);
            AssertHelper.AreEqual(ptableSrc.PreserveFormatting, ptableDest.PreserveFormatting, info + &quot;.PreserveFormatting&quot;);
            AssertHelper.AreEqual(ptableSrc.PrintTitles, ptableDest.PrintTitles, info + &quot;.PrintTitles&quot;);
            PivotFieldsTest.Property_IsSelected(ptableSrc.RowFields, ptableDest.RowFields, info + &quot;.RowFields&quot;);
            AssertHelper.AreEqual(ptableSrc.ShowRowGrandTotals, ptableDest.ShowRowGrandTotals, info + &quot;.RowGrand&quot;);
            CellAreaTest.Property_IsSelected(ptableSrc.RowRange, ptableDest.RowRange, info + &quot;.RowRange&quot;);
            AssertHelper.AreEqual(ptableSrc.SaveData, ptableDest.SaveData, info + &quot;.SaveData&quot;);
            AssertHelper.AreEqual(ptableSrc.SubtotalHiddenPageItems, ptableDest.SubtotalHiddenPageItems, info + &quot;.SubtotalHiddenPageItems&quot;);
            CellAreaTest.Property_IsSelected(ptableSrc.TableRange1, ptableDest.TableRange1, info + &quot;.TableRange1&quot;);
            CellAreaTest.Property_IsSelected(ptableSrc.TableRange2, ptableDest.TableRange2, info + &quot;.TableRange2&quot;);
            AssertHelper.AreEqual(ptableSrc.Tag, ptableDest.Tag, info + &quot;.Tag&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



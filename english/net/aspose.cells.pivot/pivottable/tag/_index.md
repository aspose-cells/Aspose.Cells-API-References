---
title: PivotTable.Tag
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a string saved with the PivotTable report
type: docs
url: /net/aspose.cells.pivot/pivottable/tag/
---
## PivotTable.Tag property

Gets a string saved with the PivotTable report.

```csharp
public string Tag { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ptableSrc.Tag, ptableDest.Tag, info + ".Tag");
public static void Property_Tag(PivotTable ptableSrc, PivotTable ptableDest, string info)
        {
            if (AssertHelper.checkNull(ptableSrc, ptableDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(ptableSrc.AutoFormatType, ptableDest.AutoFormatType, info + ".AutoFormatType");
            PivotFieldsTest.Property_Tag(ptableSrc.BaseFields, ptableDest.BaseFields, info + ".BaseFields");
            PivotFieldsTest.Property_Tag(ptableSrc.ColumnFields, ptableDest.ColumnFields, info + ".ColumnFields");
            AssertHelper.AreEqual(ptableSrc.ShowColumnGrandTotals, ptableDest.ShowColumnGrandTotals, info + ".ColumnGrand");
            CellAreaTest.Property_Tag(ptableSrc.ColumnRange, ptableDest.ColumnRange, info + ".ColumnRange");
            CellAreaTest.Property_Tag(ptableSrc.DataBodyRange, ptableDest.DataBodyRange, info + ".DataBordyRange");
            PivotFieldsTest.Property_Tag(ptableSrc.DataField, ptableDest.DataField, info + ".DataField");
            PivotFieldsTest.Property_Tag(ptableSrc.DataFields, ptableDest.DataFields, info + ".DataFields");
            AssertHelper.AreEqual(ptableSrc.DisplayErrorString, ptableDest.DisplayErrorString, info + ".DisplayErrorString");
            AssertHelper.AreEqual(ptableSrc.DisplayImmediateItems, ptableDest.DisplayImmediateItems, info + ".DisplayImmediateItems");
            AssertHelper.AreEqual(ptableSrc.DisplayNullString, ptableDest.DisplayNullString, info + ".DisplayNullString");
            AssertHelper.AreEqual(ptableSrc.EnableDrilldown, ptableDest.EnableDrilldown, info + ".EnableDrilldown");
            AssertHelper.AreEqual(ptableSrc.EnableFieldDialog, ptableDest.EnableFieldDialog, info + ".EnableFieldDialog");
            AssertHelper.AreEqual(ptableSrc.EnableFieldList, ptableDest.EnableFieldList, info + ".EnableFieldList");
            AssertHelper.AreEqual(ptableSrc.EnableWizard, ptableDest.EnableWizard, info + ".EnableWizard");
            AssertHelper.AreEqual(ptableSrc.ErrorString, ptableDest.ErrorString, info + ".ErrorString");
            AssertHelper.AreEqual(ptableSrc.IsAutoFormat, ptableDest.IsAutoFormat, info + ".IsAutoFormat");
            AssertHelper.AreEqual(ptableSrc.IsSelected, ptableDest.IsSelected, info + ".IsSelected");
            AssertHelper.AreEqual(ptableSrc.ManualUpdate, ptableDest.ManualUpdate, info + ".ManualUpdate");
            AssertHelper.AreEqual(ptableSrc.MergeLabels, ptableDest.MergeLabels, info + ".MergeLabels");
            AssertHelper.AreEqual(ptableSrc.Name, ptableDest.Name, info + ".Name");
            AssertHelper.AreEqual(ptableSrc.NullString, ptableDest.NullString, info + ".NullString");
            AssertHelper.AreEqual(ptableSrc.PageFieldOrder, ptableDest.PageFieldOrder, info + ".PageFieldOrder");
            PivotFieldsTest.Property_Tag(ptableSrc.PageFields, ptableDest.PageFields, info + ".PageFields");
            AssertHelper.AreEqual(ptableSrc.PageFieldWrapCount, ptableDest.PageFieldWrapCount, info + ".PageFieldWrapCount");
            AssertHelper.AreEqual(ptableSrc.PreserveFormatting, ptableDest.PreserveFormatting, info + ".PreserveFormatting");
            AssertHelper.AreEqual(ptableSrc.PrintTitles, ptableDest.PrintTitles, info + ".PrintTitles");
            PivotFieldsTest.Property_Tag(ptableSrc.RowFields, ptableDest.RowFields, info + ".RowFields");
            AssertHelper.AreEqual(ptableSrc.ShowRowGrandTotals, ptableDest.ShowRowGrandTotals, info + ".RowGrand");
            CellAreaTest.Property_Tag(ptableSrc.RowRange, ptableDest.RowRange, info + ".RowRange");
            AssertHelper.AreEqual(ptableSrc.SaveData, ptableDest.SaveData, info + ".SaveData");
            AssertHelper.AreEqual(ptableSrc.SubtotalHiddenPageItems, ptableDest.SubtotalHiddenPageItems, info + ".SubtotalHiddenPageItems");
            CellAreaTest.Property_Tag(ptableSrc.TableRange1, ptableDest.TableRange1, info + ".TableRange1");
            CellAreaTest.Property_Tag(ptableSrc.TableRange2, ptableDest.TableRange2, info + ".TableRange2");
            AssertHelper.AreEqual(ptableSrc.Tag, ptableDest.Tag, info + ".Tag");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



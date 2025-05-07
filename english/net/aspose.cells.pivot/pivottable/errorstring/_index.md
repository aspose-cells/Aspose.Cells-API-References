---
title: PivotTable.ErrorString
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string
type: docs
url: /net/aspose.cells.pivot/pivottable/errorstring/
---
## PivotTable.ErrorString property

Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.

```csharp
public string ErrorString { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ptableSrc.ErrorString, ptableDest.ErrorString, info + ".ErrorString");
public static void Property_ErrorString(PivotTable ptableSrc, PivotTable ptableDest, string info)
        {
            if (AssertHelper.checkNull(ptableSrc, ptableDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(ptableSrc.AutoFormatType, ptableDest.AutoFormatType, info + ".AutoFormatType");
            PivotFieldsTest.Property_ErrorString(ptableSrc.BaseFields, ptableDest.BaseFields, info + ".BaseFields");
            PivotFieldsTest.Property_ErrorString(ptableSrc.ColumnFields, ptableDest.ColumnFields, info + ".ColumnFields");
            AssertHelper.AreEqual(ptableSrc.ShowColumnGrandTotals, ptableDest.ShowColumnGrandTotals, info + ".ColumnGrand");
            CellAreaTest.Property_ErrorString(ptableSrc.ColumnRange, ptableDest.ColumnRange, info + ".ColumnRange");
            CellAreaTest.Property_ErrorString(ptableSrc.DataBodyRange, ptableDest.DataBodyRange, info + ".DataBordyRange");
            PivotFieldsTest.Property_ErrorString(ptableSrc.DataField, ptableDest.DataField, info + ".DataField");
            PivotFieldsTest.Property_ErrorString(ptableSrc.DataFields, ptableDest.DataFields, info + ".DataFields");
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
            PivotFieldsTest.Property_ErrorString(ptableSrc.PageFields, ptableDest.PageFields, info + ".PageFields");
            AssertHelper.AreEqual(ptableSrc.PageFieldWrapCount, ptableDest.PageFieldWrapCount, info + ".PageFieldWrapCount");
            AssertHelper.AreEqual(ptableSrc.PreserveFormatting, ptableDest.PreserveFormatting, info + ".PreserveFormatting");
            AssertHelper.AreEqual(ptableSrc.PrintTitles, ptableDest.PrintTitles, info + ".PrintTitles");
            PivotFieldsTest.Property_ErrorString(ptableSrc.RowFields, ptableDest.RowFields, info + ".RowFields");
            AssertHelper.AreEqual(ptableSrc.ShowRowGrandTotals, ptableDest.ShowRowGrandTotals, info + ".RowGrand");
            CellAreaTest.Property_ErrorString(ptableSrc.RowRange, ptableDest.RowRange, info + ".RowRange");
            AssertHelper.AreEqual(ptableSrc.SaveData, ptableDest.SaveData, info + ".SaveData");
            AssertHelper.AreEqual(ptableSrc.SubtotalHiddenPageItems, ptableDest.SubtotalHiddenPageItems, info + ".SubtotalHiddenPageItems");
            CellAreaTest.Property_ErrorString(ptableSrc.TableRange1, ptableDest.TableRange1, info + ".TableRange1");
            CellAreaTest.Property_ErrorString(ptableSrc.TableRange2, ptableDest.TableRange2, info + ".TableRange2");
            AssertHelper.AreEqual(ptableSrc.Tag, ptableDest.Tag, info + ".Tag");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



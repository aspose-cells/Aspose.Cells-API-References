---
title: PivotTable.AllowMultipleFiltersPerField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them
type: docs
url: /net/aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/
---
## PivotTable.AllowMultipleFiltersPerField property

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(pt.AllowMultipleFiltersPerField);
[Test]
        public void Property_AllowMultipleFiltersPerField()
        {
            var wb = new Workbook(Constants.openPivottablePath + "testPivotTableOptions.xlsx");
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            Assert.AreEqual(pt.PageFieldWrapCount,2);
            Assert.AreEqual(pt.DisplayNullString,false);
            Assert.AreEqual(pt.PreserveFormatting,false);
           // Assert.AreEqual(pt.RepeatItemsOnEachPrintedPage,false);
            Assert.AreEqual(pt.PrintTitles, false);
            Assert.AreEqual(pt.EnableFieldList,true);
            Assert.IsFalse(pt.DisplayNullString);
            Assert.IsFalse(pt.DisplayErrorString);
            Assert.IsFalse(pt.MergeLabels);
            Assert.AreEqual(2,pt.PageFieldWrapCount);
            Assert.IsTrue(pt.ShowColumnGrandTotals);
            Assert.IsTrue(pt.ShowRowGrandTotals);
            Assert.IsTrue(pt.CustomListSort);
            Assert.IsTrue(pt.EnableDrilldown);
            Assert.IsTrue(pt.ShowDataTips);
            Assert.IsTrue(pt.ShowDrill);
            Assert.IsFalse(pt.ShowValuesRow);
            Assert.IsFalse(pt.IsGridDropZones);
            Assert.IsFalse(pt.AllowMultipleFiltersPerField);
            Assert.IsTrue(pt.ShowRowHeaderCaption);
            wb.Save(Constants.savePivottablePath + "40114.xlsx");

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



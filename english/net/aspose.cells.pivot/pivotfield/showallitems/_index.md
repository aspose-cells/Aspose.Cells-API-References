---
title: PivotField.ShowAllItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether all items displays in the PivotTable report even if they dont contain summary data. show items with no data The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

```csharp
public bool ShowAllItems { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].BaseFields[0].ShowAllItems);
[Test]
        public void Property_ShowAllItems()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56933.xlsx");
            Workbook a = new Workbook();
            a.Copy(workbook);
           Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].BaseFields[0].ShowAllItems);
            Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].BaseFields[0].IsRepeatItemLabels);
            a.Save(Constants.PivotTableDestPath + "CELLSNET56933.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: PivotTable.MergeLabels
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. True if the specified PivotTable reports outerrow item column item subtotal and grand total labels use merged cells
type: docs
url: /net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

True if the specified PivotTable report's outer-row item, column item, subtotal, and grand total labels use merged cells.

```csharp
public bool MergeLabels { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].PivotTables[0].MergeLabels = true;
[Test]
        public void Property_MergeLabels()
        {

            Workbook wb = new Workbook(Constants.openPivottablePath + "aa.xlsx");
            wb.Worksheets[0].PivotTables[0].MergeLabels = true;
            wb.Save(Constants.savePivottablePath + "aa.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



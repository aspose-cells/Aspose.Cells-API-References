---
title: PivotTable.CalculateRange
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables range
type: docs
url: /net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Calculates pivottable's range.

```csharp
public void CalculateRange()
```

### Remarks

If this method is not been called,maybe the pivottable range is not corrected.

### Examples

```csharp
// Called: pt1.CalculateRange();
[Test]
        public void Method_CalculateRange()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46016_";

            Workbook workbook = new Workbook(filePath + "testsheet.xlsx");
            Worksheet sheetOverview = workbook.Worksheets["Overview"];
            PivotTable pt1 = sheetOverview.PivotTables["PivotTable1"];
            pt1.RefreshData();
            pt1.CalculateData();
            pt1.CalculateRange();
            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + "NET46016.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



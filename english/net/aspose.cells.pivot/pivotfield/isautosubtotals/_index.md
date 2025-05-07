---
title: PivotField.IsAutoSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field shows automatic subtotals. Default is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Indicates whether the specified field shows automatic subtotals. Default is true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[2].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
[Test]
        public void Property_IsAutoSubtotals()
        {

            Workbook wb = new Workbook(Constants.openPivottablePath + "Source.xlsx");
            Style style = wb.CreateStyle();
            style.Custom = "dd/mmm";
            wb.Worksheets[2].PivotTables[0].Format(9, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(10, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(11, 0, style);
            wb.Worksheets[2].PivotTables[0].Format(12, 0, style);
            wb.Worksheets[2].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
            wb.Worksheets[2].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
            wb.Worksheets[2].PivotTables[0].RefreshData();
            wb.Worksheets[2].PivotTables[0].CalculateData();
            wb.Save(Constants.savePivottablePath + "40013.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



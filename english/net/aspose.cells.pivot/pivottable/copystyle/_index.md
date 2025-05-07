---
title: PivotTable.CopyStyle
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Copies named style from another pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Copies named style from another pivot table.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Source pivot table. |

### Examples

```csharp
// Called: wb1.Worksheets[0].PivotTables[0].CopyStyle(wb.Worksheets[0].PivotTables[0]);
[Test]
        public void Method_PivotTable_()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + "svxBoardPaper.xlsm");
            Workbook wb1 = new Workbook(Constants.openPivottablePath + "eeee.xlsx");
            wb1.Worksheets[0].PivotTables[0].CopyStyle(wb.Worksheets[0].PivotTables[0]);
            wb1.Save(Constants.savePivottablePath + "40331.xlsx");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



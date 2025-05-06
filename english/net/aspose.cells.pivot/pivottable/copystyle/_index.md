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
            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;svxBoardPaper.xlsm&quot;);
            Workbook wb1 = new Workbook(Constants.openPivottablePath + &quot;eeee.xlsx&quot;);
            wb1.Worksheets[0].PivotTables[0].CopyStyle(wb.Worksheets[0].PivotTables[0]);
            wb1.Save(Constants.savePivottablePath + &quot;40331.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: PivotTable.PivotTableStyleType
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the builtin pivot table style
type: docs
url: /net/aspose.cells.pivot/pivottable/pivottablestyletype/
---
## PivotTable.PivotTableStyleType property

Gets and sets the built-in pivot table style.

```csharp
public PivotTableStyleType PivotTableStyleType { get; set; }
```

### Examples

```csharp
// Called: pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
private PivotTable Property_PivotTableStyleType(Workbook book)
        {
            Worksheet sheet = book.Worksheets[0];
            PivotTableCollection pivots = sheet.PivotTables;

            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            return pivot;
        }
```

### See Also

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



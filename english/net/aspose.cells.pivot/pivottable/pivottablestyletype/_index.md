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
// Called: PivotTableStyleType type = wb.Worksheets[0].PivotTables[0].PivotTableStyleType;
public void PivotTable_Property_PivotTableStyleType()
{
    string filePath = Constants.PivotTableSourcePath + @"NET51306_";
    string savePath = CreateFolder(filePath);
    Workbook workbook = new Workbook(filePath + @"test.xlsx");
    Workbook newWorkbook = new Workbook();
    newWorkbook.Copy(workbook);
    newWorkbook.Save(savePath + "out.xlsx");

    Workbook wb = new Workbook(savePath + "out.xlsx");
    PivotTableStyleType type = wb.Worksheets[0].PivotTables[0].PivotTableStyleType;
    Assert.AreEqual(type, PivotTableStyleType.None);
}
```

### See Also

* enum [PivotTableStyleType](../../pivottablestyletype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: PivotTable.IsGridDropZones
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable report displays classic pivottable layout. enables dragging fields in the grid
type: docs
url: /net/aspose.cells.pivot/pivottable/isgriddropzones/
---
## PivotTable.IsGridDropZones property

Indicates whether the PivotTable report displays classic pivottable layout. (enables dragging fields in the grid)

```csharp
public bool IsGridDropZones { get; set; }
```

### Examples

```csharp
// Called: bool first = wb.Worksheets["Report"].PivotTables[0].IsGridDropZones;
public void PivotTable_Property_IsGridDropZones()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA41530_";

    Workbook wb = new Workbook(filePath + "pivot.xlsb");
    bool first = wb.Worksheets["Report"].PivotTables[0].IsGridDropZones;
    wb.Save(Constants.PivotTableDestPath + @"example.xlsb");

    wb = new Workbook(Constants.PivotTableDestPath + @"example.xlsb");
    Assert.AreEqual(first, wb.Worksheets["Report"].PivotTables[0].IsGridDropZones);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



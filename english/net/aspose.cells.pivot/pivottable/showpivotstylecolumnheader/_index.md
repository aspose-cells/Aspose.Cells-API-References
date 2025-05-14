---
title: PivotTable.ShowPivotStyleColumnHeader
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the column header in the pivot table should have the style applied
type: docs
url: /net/aspose.cells.pivot/pivottable/showpivotstylecolumnheader/
---
## PivotTable.ShowPivotStyleColumnHeader property

Indicates whether the column header in the pivot table should have the style applied.

```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(pt.ShowPivotStyleColumnHeader, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleColumnHeader);
public void PivotTable_Property_ShowPivotStyleColumnHeader()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43735_";
    Workbook wb_a = new Workbook(filePath + "wbA.xlsx");
    Workbook wb_b = new Workbook(filePath + "wbB.xlsx");
    wb_a.Combine(wb_b);
    wb_a.Save(Constants.PivotTableDestPath + "example.xlsx");

    Workbook wb = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    PivotTable pt = wb.Worksheets["SheetB"].PivotTables["PivotTable1"];
    Assert.AreEqual(pt.ShowPivotStyleRowStripes, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleRowStripes);
    Assert.AreEqual(pt.ShowPivotStyleColumnStripes, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleColumnStripes);
    Assert.AreEqual(pt.ShowPivotStyleRowHeader, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleRowHeader);
    Assert.AreEqual(pt.ShowPivotStyleColumnHeader, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleColumnHeader);
    Assert.AreEqual(pt.ShowPivotStyleLastColumn, wb_b.Worksheets["SheetB"].PivotTables["PivotTable1"].ShowPivotStyleLastColumn);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



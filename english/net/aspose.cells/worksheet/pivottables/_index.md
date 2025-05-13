---
title: Worksheet.PivotTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all pivot tables in this worksheet
type: docs
url: /net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Gets all pivot tables in this worksheet.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Examples

```csharp
// Called: Aspose.Cells.Pivot.PivotTable _PivotTable = _sheetActiva.PivotTables[0];
public void Worksheet_Property_PivotTables()
{
    string filePath = Constants.PivotTableSourcePath + @"NET44514_";

    Workbook workbook = new Workbook(filePath + "SellOut.xlsx");
    Aspose.Cells.Worksheet _sheetActiva = workbook.Worksheets[0];

    //aplicar filtro
    Aspose.Cells.Pivot.PivotTable _PivotTable = _sheetActiva.PivotTables[0];

    _PivotTable.PivotFilters.Clear();

    Aspose.Cells.Pivot.PivotField _PivotField = GetPivotFieldByDisplayNameNET44514(ref _PivotTable, "Ejercicio");

    List<string> _lstStrValores = new List<string>() { "2014/15" };
    SetValuePivotFieldNET44514(ref _sheetActiva, ref _PivotTable, ref _PivotField, _lstStrValores);


    workbook.Save(Constants.PivotTableDestPath + @"example.xlsx");
}
```

### See Also

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



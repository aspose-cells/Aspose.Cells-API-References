---
title: PivotTable.GetCellByDisplayName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the Cell object by the display name of PivotField
type: docs
url: /net/aspose.cells.pivot/pivottable/getcellbydisplayname/
---
## PivotTable.GetCellByDisplayName method

Gets the [`Cell`](../../../aspose.cells/cell/) object by the display name of PivotField.

```csharp
public Cell GetCellByDisplayName(string displayName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| displayName | String | the DisplayName of PivotField |

### Return Value

the Cell object

### Examples

```csharp
// Called: Cell cell = pivotTable.GetCellByDisplayName(displayName);
public void PivotTable_Method_GetCellByDisplayName()
{
    string filePath = Constants.PivotTableSourcePath  + @"NET44304_";
    Workbook wb = new Workbook(filePath + "sample.xlsx");
    Worksheet ws = wb.Worksheets["Pivot Sheet"];

    PivotTable pivotTable = ws.PivotTables[0];

    pivotTable.IsExcel2003Compatible = false;
    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = false;

    var dataFields = pivotTable.Fields(PivotFieldType.Data);

    for (int i = 255; i < dataFields.Count; i++)
    {
        var displayName = dataFields[i].DisplayName;

        Cell cell = pivotTable.GetCellByDisplayName(displayName);

        if (cell == null)
        {
            Assert.Fail("find null via PivotField.DisplayName");
            Console.WriteLine(displayName + "----Null");
        }
        else
        {
            Console.WriteLine(displayName + "----" + cell.Name);
        }
    }
    wb.Save(Constants.PivotTableDestPath + @"example.xlsx");

    wb = new Workbook(Constants.PivotTableDestPath + @"example.xlsx");
    pivotTable = wb.Worksheets["Pivot Sheet"].PivotTables[0];
    dataFields = pivotTable.Fields(PivotFieldType.Data);
    for (int i = 255; i < dataFields.Count; i++)
    {
        var displayName = dataFields[i].DisplayName;

        Cell cell = pivotTable.GetCellByDisplayName(displayName);

        if (cell == null)
        {
            Assert.Fail("find null via PivotField.DisplayName");
            Console.WriteLine(displayName + "----Null");
        }
        else
        {
            Console.WriteLine(displayName + "----" + cell.Name);
        }
    }
}
```

### See Also

* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: Cells.MaxDataColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of cell which contains data
type: docs
url: /net/aspose.cells/cells/maxdatacolumn/
---
## Cells.MaxDataColumn property

Maximum column index of cell which contains data.

```csharp
public int MaxDataColumn { get; }
```

### Remarks

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet, so it is a time-consumed progress and should not be invoked repeatedly.

### Examples

```csharp
// Called: var data = dataSheet.Cells.ExportDataTable(0, 0, dataSheet.Cells.MaxDataRow + 1, dataSheet.Cells.MaxDataColumn + 1);
public void Cells_Property_MaxDataColumn()
{
    string filePath = Constants.PivotTableSourcePath + @"NET44089_";
    var book = new Workbook(filePath + "output%2b(6).xlsm");
    var dataSheet = book.Worksheets["Sheet1"];
    var data = dataSheet.Cells.ExportDataTable(0, 0, dataSheet.Cells.MaxDataRow + 1, dataSheet.Cells.MaxDataColumn + 1);
    var pivotData = book.Worksheets["Hoja3"];
    pivotData.Cells.ImportData(data, 0, 0, new ImportTableOptions() { IsFieldNameShown = false });
    foreach (Aspose.Cells.Worksheet worksheet in book.Worksheets)
    {
        //worksheet.RefreshPivotTables(); //throws same error
        foreach (Aspose.Cells.Pivot.PivotTable pivotTable in worksheet.PivotTables)
        {
            //pivotTable.RefreshDataOnOpeningFile = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData(); //Error
            pivotTable.RefreshDataOnOpeningFile = false;
        }
    }
    book.Save(Constants.PivotTableDestPath + @"example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: Cells.ImportDataView
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports a DataView into a worksheet
type: docs
url: /net/aspose.cells/cells/importdataview/
---
## Cells.ImportDataView method

Imports a DataView into a worksheet.

```csharp
public int ImportDataView(DataView dataView, int firstRow, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataView | DataView | The DataView object to be imported. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### Return Value

Total number of rows imported

### Examples

```csharp
// Called: cells.ImportDataView(dataview, 0, 255);
public void Cells_Method_ImportDataView()
{
    caseName = "testDataView_003";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    DataView dataview = getDataView();
    cells.ImportDataView(dataview, 0, 255);

    checkImportDataView_003(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    //workbook.Save(Constants.destPath + "testDataView.xls");            
    //workbook = new Workbook(Constants.destPath + "testDataView.xls");
    checkImportDataView_003(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath + "testDataView.xlsx");            
    //workbook = new Workbook(Constants.destPath + "testDataView.xlsx");
    checkImportDataView_003(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    //workbook.Save(Constants.destPath + "testDataView.xml", SaveFormat.SpreadsheetML);
    //workbook = new Workbook(Constants.destPath + "testDataView.xml");
    checkImportDataView_003(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    //workbook.Save(Constants.destPath + "testDataView.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



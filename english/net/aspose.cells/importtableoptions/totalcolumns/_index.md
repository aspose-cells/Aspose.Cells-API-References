---
title: ImportTableOptions.TotalColumns
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets total column count to import from data source. 1 means all rows of given data source
type: docs
url: /net/aspose.cells/importtableoptions/totalcolumns/
---
## ImportTableOptions.TotalColumns property

Gets or sets total column count to import from data source. -1 means all rows of given data source.

```csharp
public int TotalColumns { get; set; }
```

### Examples

```csharp
// Called: { IsFieldNameShown = true, InsertRows = true, TotalRows = 1, TotalColumns = 2 });
public void ImportTableOptions_Property_TotalColumns()
{
    caseName = "testImportDataTable_016";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    DataTable datatable = getDataTable();
    cells[0, 0].PutValue(1);
    cells.ImportData(datatable, 0, 0, new ImportTableOptions()
    { IsFieldNameShown = true, InsertRows = true, TotalRows = 1, TotalColumns = 2 });

    checkImportDataTable_016(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    //workbook.Save(Constants.destPath + "testImportDataTable.xls");
    //workbook = new Workbook(Constants.destPath + "testImportDataTable.xls");
    checkImportDataTable_016(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    //workbook.Save(Constants.destPath + "testImportDataTable.xlsx");
    //workbook = new Workbook(Constants.destPath + "testImportDataTable.xlsx");
    checkImportDataTable_016(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.SpreadsheetML);
    //workbook.Save(Constants.destPath + "testImportDataTable.xml", SaveFormat.SpreadsheetML);
    //workbook = new Workbook(Constants.destPath + "testImportDataTable.xml");
    checkImportDataTable_016(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    //workbook.Save(Constants.destPath + "testImportDataTable.xls"); 
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



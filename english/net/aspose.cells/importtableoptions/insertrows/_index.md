---
title: ImportTableOptions.InsertRows
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether new rows should be added for importing data records
type: docs
url: /net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Indicates whether new rows should be added for importing data records.

```csharp
public bool InsertRows { get; set; }
```

### Examples

```csharp
// Called: options.InsertRows = true;
public void ImportTableOptions_Property_InsertRows()
{
    caseName = "testImportDataColumn_001";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    DataTable datatable = getDataTable();
    cells[0, 0].PutValue(1);
    ImportTableOptions options = new ImportTableOptions();
    options.ColumnIndexes = new int[] { 2 };
    options.InsertRows = true;
    options.IsFieldNameShown = true;

    cells.ImportData(datatable, 0,0,options);

    checkImportDataColumn_001(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xls");            
    workbook = new Workbook(Constants.destPath + "testImportDataColumn.xls");
    checkImportDataColumn_001(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xlsx");
    workbook = new Workbook(Constants.destPath + "testImportDataColumn.xlsx");
    checkImportDataColumn_001(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testImportDataColumn.xml");
    checkImportDataColumn_001(workbook);
    workbook.Save(Constants.destPath + "testImportDataColumn.xls"); 
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: ImportTableOptions.ColumnIndexes
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Gets or sets the columns0based to import from data source. null means all columns should be imported
type: docs
url: /net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Examples

```csharp
// Called: options.ColumnIndexes = new int[] { 2 };
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void ImportTableOptions_Property_ColumnIndexes()
        {
            caseName = "testImportDataColumn_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable();

            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 2 };
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            cells.ImportData(datatable, -1, 0, options);
            string msg = message + "cells.ImportDataColumn(datatable, true, -1, 0, 2, true)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



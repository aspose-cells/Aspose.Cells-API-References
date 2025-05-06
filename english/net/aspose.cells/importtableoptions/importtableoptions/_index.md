---
title: ImportTableOptions.ImportTableOptions
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions constructor. Creates the default importing options
type: docs
url: /net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Creates the default importing options.

```csharp
public ImportTableOptions()
```

### Examples

```csharp
// Called: cells.ImportData(datatable, 1048576, 0, new ImportTableOptions() { IsFieldNameShown = true });
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void ImportTableOptions_Constructor()
        {
            caseName = &quot;testImportDataTable_Exception_003&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            DataTable datatable = getDataTable();
            cells.ImportData(datatable, 1048576, 0, new ImportTableOptions() { IsFieldNameShown = true });
            string msg = message + &quot;cells.ImportDataTable(datatable, true, 1048576, 0)&quot;;
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



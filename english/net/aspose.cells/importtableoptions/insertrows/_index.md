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
// Called: { IsFieldNameShown = true, InsertRows = true, TotalRows = tbl.Rows.Count, TotalColumns = tbl.Columns.Count });
public static void Property_InsertRows()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Workbook workbook = new Workbook(USBankConstants.sourcePath + "ImportDataTable.xlsx");
            designer.Workbook = workbook;

            Cells sourceCells = workbook.Worksheets[0].Cells;
            DataTable tbl = CreateValidTable1();

            sourceCells.ImportData(tbl, 0, 0, new ImportTableOptions()
            { IsFieldNameShown = true, InsertRows = true, TotalRows = tbl.Rows.Count, TotalColumns = tbl.Columns.Count });
            string output = USBankConstants.resultPath + "ImportDataTable_result.xlsx";
            workbook.Save(output);
        }
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



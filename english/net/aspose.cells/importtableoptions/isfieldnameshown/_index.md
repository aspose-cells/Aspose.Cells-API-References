---
title: ImportTableOptions.IsFieldNameShown
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether field name should be imported
type: docs
url: /net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Indicates whether field name should be imported.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Examples

```csharp
// Called: cells.ImportData(table, 8, 0, new ImportTableOptions() { IsFieldNameShown = true, InsertRows = true });
public void ImportTableOptions_Property_IsFieldNameShown()
{
    DataTable table = new DataTable();
    table.Columns.Add("Id");
    table.Columns.Add("Name");
            
    for (int i = 0; i < 10; i++)
    {
        DataRow row = table.Rows.Add();
        row[0] = i;
        row[1] = "Name" + i;
    }
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells["A10"].PutValue("A10");
    cells.ImportData(table, 8, 0, new ImportTableOptions() { IsFieldNameShown = true, InsertRows = true });
    workbook.Save(Constants.destPath + "ImportDataTable.xls");
            
}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



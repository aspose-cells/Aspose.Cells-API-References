---
title: Cells.InsertColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts a new column into the worksheet
type: docs
url: /net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Inserts a new column into the worksheet.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |

### Examples

```csharp
// Called: cells.InsertColumn(colIndex + 1, true);
protected static void Cells_Method_InsertColumn(Worksheet sheet, int colIndex, int qtyColumns)
        {
            // colIndex is the source column for the set of columns that will be created.
            Cells cells = sheet.Cells;
            for (int i = 1; i < qtyColumns; i++)
                cells.InsertColumn(colIndex + 1, true);

            // copy the first column across the entire metric range...
            for (int i = 1; i < qtyColumns; i++)
                cells.CopyColumn(cells, colIndex, colIndex + i);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Inserts a new column into the worksheet.

```csharp
public void InsertColumn(int columnIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |

### Examples

```csharp
// Called: cells.InsertColumn(2);
public void Cells_Method_InsertColumn()
{
    caseName = "testInsertChart_010";
    Workbook workbook = new Workbook();
    workbook = new Workbook(Constants.sourcePath + "insertDelete\\insertSourceData.xls");
    Worksheet sheet = workbook.Worksheets[0];
    Cells cells = sheet.Cells;
    Chart chart = sheet.Charts[0];
    cells.InsertRow(3);
    cells.InsertColumn(2);

    checkInsertChart_010(workbook);
    workbook.Save(Constants.destPath + " testInsertChart.xls");
    workbook = new Workbook(Constants.destPath + " testInsertChart.xls");
    checkInsertChart_010(workbook);
    workbook.Save(Constants.destPath + " testInsertChart.xlsx");
    workbook = new Workbook(Constants.destPath + " testInsertChart.xlsx");
    checkInsertChart_010(workbook);
    workbook.Save(Constants.destPath + " testInsertChart.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



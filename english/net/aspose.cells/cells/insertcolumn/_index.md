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
protected static void Method_Boolean_(Worksheet sheet, int colIndex, int qtyColumns)
        {
            // colIndex is the source column for the set of columns that will be created.
            Cells cells = sheet.Cells;
            for (int i = 1; i &lt; qtyColumns; i++)
                cells.InsertColumn(colIndex + 1, true);

            // copy the first column across the entire metric range...
            for (int i = 1; i &lt; qtyColumns; i++)
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
// Called: cells.InsertColumn(0);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testInsertChart_008&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\insertSourceData.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            Chart chart = sheet.Charts[0];
            cells.InsertRow(0);
            cells.InsertColumn(0);

            checkInsertChart_008(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xls&quot;);
            
            workbook = new Workbook(Constants.destPath + &quot; testInsertChart.xls&quot;);
            checkInsertChart_008(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xlsx&quot;);            
            workbook = new Workbook(Constants.destPath + &quot; testInsertChart.xlsx&quot;);
            checkInsertChart_008(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



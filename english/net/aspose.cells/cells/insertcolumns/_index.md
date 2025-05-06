---
title: Cells.InsertColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts some columns into the worksheet
type: docs
url: /net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |

### Examples

```csharp
// Called: cells.InsertColumns(0, 2);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testInsertChart_005&quot;;
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\insertSourceData.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            Chart chart = sheet.Charts[0];
            cells.InsertColumn(0);
            cells.InsertColumns(0, 2);

            checkInsertChart_005(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testInsertChart.xls&quot;);
            checkInsertChart_005(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testInsertChart.xlsx&quot;);
            checkInsertChart_005(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertChart.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |

### Examples

```csharp
// Called: workbook.Worksheets[&amp;quot;Daily Data&amp;quot;].Cells.InsertColumns(7, 3, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;110+Viking+Daily.xls&quot;);
            workbook.Worksheets[&quot;Daily Data&quot;].Cells.InsertColumns(7, 3, true);


        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

Inserts some columns into the worksheet.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| options | InsertOptions | The options for inserting operation. |

### See Also

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



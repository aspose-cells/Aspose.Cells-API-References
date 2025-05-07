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
// Called: cells.InsertColumn(0, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ChartsUpdateOtherRef.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertColumn(0, true);
            cells.InsertRows(0, 10, true);
            cells.DeleteColumn(0, true);
            cells.DeleteRows(0, 5, true);
           // 
            Assert.AreEqual(workbook.Worksheets[2].Charts[0].NSeries[0].Values, workbook.Worksheets[0].Charts[0].NSeries[0].Values);
            workbook.Save(Constants.destPath + "ChartsUpdateOtherRef.xls");
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
// Called: cells.InsertColumn(1);
[Test]
        public void Method_Int32_()
        {
            caseName = "testInsertFormual_008";
            Workbook workbook = new Workbook(Constants.sourcePath + "insertDelete\\testformual.xls");
            checkInsertFormual(workbook);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertColumn(1);

            checkInsertFormual_008(workbook);
            workbook.Save(Constants.destPath + "testInsertFormual.xls");
            workbook = new Workbook(Constants.destPath + "testInsertFormual.xls");
            checkInsertFormual_008(workbook);
            workbook.Save(Constants.destPath + "testInsertFormual.xlsx");
            workbook = new Workbook(Constants.destPath + "testInsertFormual.xlsx");
            checkInsertFormual_008(workbook);
            workbook.Save(Constants.destPath + "testInsertFormual.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testInsertFormual.xml");
            checkInsertFormual_008(workbook);
            workbook.Save(Constants.destPath + "testInsertFormual.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: Cells.InsertRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Inserts multiple rows into the worksheet
type: docs
url: /net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Inserts multiple rows into the worksheet.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |

### Examples

```csharp
// Called: worksheet.Cells.InsertRows(2, 2, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            worksheet.Cells.InsertRows(2, 2, true);
            Assert.AreEqual(5, cellRange.RowCount);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Inserts multiple rows into the worksheet.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |
| options | InsertOptions | Options for inserting operation. |

### Examples

```csharp
// Called: worksheet.Cells.InsertRows(5, 3, insertOptions);
public static void Method_InsertOptions_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an instance of InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Define the cell area where rows will be inserted
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Insert rows with the specified options
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Save the workbook
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
```

### See Also

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Inserts multiple rows into the worksheet.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |

### Examples

```csharp
// Called: cells.InsertRows(0, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Copy\\hide_001.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertRows(0, 2);

            CheckInsertRows_HideRowAndColumn_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRows.xls");
            workbook = new Workbook(Constants.destPath + " testInsertRows.xls");
            CheckInsertRows_HideRowAndColumn_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRows.xlsx");
            workbook = new Workbook(Constants.destPath + " testInsertRows.xlsx");
            CheckInsertRows_HideRowAndColumn_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRows.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + " testInsertRows.xml");
            CheckInsertRows_HideRowAndColumn_001(workbook);
            workbook.Save(Constants.destPath + " testInsertRows.xls");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



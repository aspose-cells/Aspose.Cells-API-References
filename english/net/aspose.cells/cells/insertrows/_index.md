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
// Called: cells.InsertRows(10, 2000, true);
[Test]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Test_176053.xls&quot;);
            Cells cells = workbook.Worksheets[1].Cells;
            cells.InsertRows(10, 2000, true);
            for (int i = 10; i &lt; 2000; i++)
            {
               cells.CopyRow(workbook.Worksheets[1].Cells, 9, i);
            }
            Assert.AreEqual(cells[&quot;B11&quot;].Formula, &quot;=Sheet1!B2&quot;);
            Assert.AreEqual(cells[&quot;C11&quot;].Formula, &quot;=SUM(Sheet1!C2:D2)&quot;);
            Util.ReSave(workbook, SaveFormat.Excel97To2003);
            //workbook.Save(Constants.destPath + &quot;Test_176053.xls&quot;);
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
            workbook.Save(&quot;InsertOptionsExample.xlsx&quot;);
            workbook.Save(&quot;InsertOptionsExample.pdf&quot;);
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
// Called: cells.InsertRows(5, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
          workbook = new Workbook(Constants.sourcePath + &quot;insertDelete\\testStyle.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertRows(5, 2);

            CheckInsertRows_Style_002(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertRows.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testInsertRows.xls&quot;);
            CheckInsertRows_Style_002(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertRows.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testInsertRows.xlsx&quot;);
            CheckInsertRows_Style_002(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertRows.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot; testInsertRows.xml&quot;);
            CheckInsertRows_Style_002(workbook);
            workbook.Save(Constants.destPath + &quot; testInsertRows.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



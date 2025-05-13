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
// Called: worksheet.Cells.InsertRows(11, 1, true);
public void Cells_Method_InsertRows()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "BudgetExportTemplate+AlmostFinal.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    worksheet.Cells.InsertRows(11, 1, true);
    Assert.AreEqual(worksheet.Cells["D12"].Formula, "=F12-E12");
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
public static void Cells_Method_InsertRows()
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
// Called: cells.InsertRows(4, 2);
// Is there away to insert rows to an existing ListObject? 
// http://www.aspose.com/community/forums/thread/296251.aspx
public void Cells_Method_InsertRows()
{
    Console.WriteLine("Cells_Method_InsertRows()");
    string infn = path + @"example.xlsx";
    string outfn = Constants.destPath + @"ListObectInsRows_Book1_out.xlsx";

    Workbook workbook = new Workbook(infn);
    Cells cells = workbook.Worksheets[0].Cells;

    cells.InsertRows(4, 2);
    Assert.IsNull(cells[4, 1].Value);
    workbook.Save(outfn);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



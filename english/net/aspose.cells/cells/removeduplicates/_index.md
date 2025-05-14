---
title: Cells.RemoveDuplicates
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Removes duplicate rows in the sheet
type: docs
url: /net/aspose.cells/cells/removeduplicates/
---
## RemoveDuplicates() {#removeduplicates}

Removes duplicate rows in the sheet.

```csharp
public void RemoveDuplicates()
```

### Examples

```csharp
// Called: cells.RemoveDuplicates(); //IndexOutOfRangeException
public void Cells_Method_RemoveDuplicates()
{
    Workbook wb = new Workbook();
    Style ds = wb.DefaultStyle;
    ds.Custom = "00000";
    Cells cells = wb.Worksheets[0].Cells;
    bool odd = false;
    for (int i = 0; i < 70; i++)
    {
        for (int j = odd ? 1 : 0; j < 10; j += 2)
        {
            cells[i, j].PutValue(i * 10 + j);
        }
        odd = !odd;
    }
    cells.RemoveDuplicates(); //IndexOutOfRangeException
    Assert.AreEqual(69, cells.MaxDataRow, "MaxDataRow");
    Assert.AreEqual(350, cells.Count, "CellCount");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int) {#removeduplicates_1}

Removes duplicate values in the range.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| endRow | Int32 | The end row index. |
| endColumn | Int32 | The end column index. |

### Examples

```csharp
// Called: cells.RemoveDuplicates(0, 0, 10, 1);
public void Cells_Method_RemoveDuplicates()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    cells.RemoveDuplicates(0, 0, 10, 1);
    Assert.AreEqual(cells["A3"].StringValue, "dd");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveDuplicates(int, int, int, int, bool, int[]) {#removeduplicates_2}

Removes duplicate data of the range.

```csharp
public void RemoveDuplicates(int startRow, int startColumn, int endRow, int endColumn, 
    bool hasHeaders, int[] columnOffsets)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row. |
| startColumn | Int32 | The start column |
| endRow | Int32 | The end row index. |
| endColumn | Int32 | The end column index. |
| hasHeaders | Boolean | Indicates whether the range contains headers. |
| columnOffsets | Int32[] | The column offsets. |

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



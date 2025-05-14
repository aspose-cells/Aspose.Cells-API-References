---
title: ListObjectCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ListObjectCollection method. Adds a ListObject to the worksheet
type: docs
url: /net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Adds a ListObject to the worksheet.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The start row of the list range. |
| startColumn | Int32 | The start row of the list range. |
| endRow | Int32 | The start row of the list range. |
| endColumn | Int32 | The start row of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |

### Return Value

The index of the new ListObject

### Examples

```csharp
// Called: worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);
public void ListObjectCollection_Method_Add()
{
    var workbook = new Workbook();
    var worksheet = workbook.Worksheets[0];

    // Populate range            
    var range = worksheet.Cells.CreateRange("B3:D4");
    range.Value = new object[,]
    {
        {"Col1","Col2","Col3" },
        {100,200,300 },
    };

    // Create ListObject
    var firstRow = range.FirstRow;
    var endRow = firstRow + range.RowCount - 1;
    var firstColumn = range.FirstColumn;
    var endColumn = firstColumn + range.ColumnCount - 1;
    worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

    // Show totals
    worksheet.ListObjects[0].ShowTotals = true;
    Assert.AreEqual("=SUBTOTAL(109,[Col3])", worksheet.Cells["D5"].Formula);
    //workbook.Save(Constants.destPath + "example.xlsx");
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
}
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Adds a ListObject to the worksheet.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startCell | String | The start cell of the list range. |
| endCell | String | The end cell of the list range. |
| hasHeaders | Boolean | Whether the range has headers. |

### Return Value

The index of the new ListObject

### Examples

```csharp
// Called: listObjects.Add("A1", "B4", false);
public void ListObjectCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue("a");
    cells[1, 0].PutValue(1);
    cells[2, 0].PutValue(2);
    cells[3, 0].PutValue(3);
    cells[0, 1].PutValue("b");
    cells[1, 1].PutValue(4);
    cells[2, 1].PutValue(5);
    cells[3, 1].PutValue(6);

    ListObjectCollection listObjects = workbook.Worksheets[0].ListObjects;
    listObjects.Add("A1", "B4", false);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)



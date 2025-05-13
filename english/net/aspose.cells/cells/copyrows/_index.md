---
title: Cells.CopyRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of some whole rows
type: docs
url: /net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |

### Examples

```csharp
// Called: cells.CopyRows(sourcecells, 0,
public void Cells_Method_CopyRows()
{
         
    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook book2 = new Workbook(Constants.sourcePath + "example.xlsx");

    //Get the first worksheet 
    Worksheet sheet = book2.Worksheets[0];

    Cells cells, sourcecells;

    cells = book.Worksheets[0].Cells;
    sourcecells = sheet.Cells;

    // copy book2's contents to book's sheet at the end 
    cells.CopyRows(sourcecells, 0,
            cells.MaxDisplayRange.RowCount + 2,
            sourcecells.MaxDisplayRange.RowCount);

    Assert.AreEqual(book.Worksheets[0].SparklineGroups.Count, 2);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1, options);
public void Cells_Method_CopyRows()
{

    Aspose.Cells.Workbook aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,2);

    aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
    aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1);
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,4);

    aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);
    CopyOptions options = new CopyOptions();
    options.ExtendToAdjacentRange = true;
    aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
    aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1, options);
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);

}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



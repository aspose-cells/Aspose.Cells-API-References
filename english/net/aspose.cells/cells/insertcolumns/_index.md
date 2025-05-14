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
// Called: workbook.Worksheets[2].Cells.InsertColumns(1, 3);
	    public void Cells_Method_InsertColumns()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
            workbook.Worksheets.AddCopy("Orig Sheet");
            workbook.Worksheets[2].Cells.InsertColumns(1, 3);
            Aspose.Cells.Range loPasteFromRange = workbook.Worksheets[2].Cells.CreateRange(0, 1, true);
            Aspose.Cells.Range loPasteToRange = workbook.Worksheets[2].Cells.CreateRange(1, 3, true);
            loPasteToRange.Copy(loPasteFromRange);
            Assert.AreEqual(1, workbook.Worksheets[2].Cells.GetMergedAreas().Length);
            Util.ReSave(workbook, SaveFormat.Xlsx);
            //workbook.Save(Constants.destPath + "example.xlsx");
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
// Called: workbook.Worksheets["Daily Data"].Cells.InsertColumns(7, 3, true);
public void Cells_Method_InsertColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Worksheets["Daily Data"].Cells.InsertColumns(7, 3, true);


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

### Examples

```csharp
// Called: worksheet.Cells.InsertColumns(3, 1, options);
public void Cells_Method_InsertColumns()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];

    InsertOptions options = new InsertOptions();
    options.CopyFormatType = CopyFormatType.Clear;

    worksheet.Cells.InsertColumns(3, 1, options);
    Cell cell = worksheet.Cells["D10"];
    Style style = cell.GetStyle(false);
    Assert.AreEqual(CellBorderType.None, style.Borders[BorderType.TopBorder].LineStyle);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



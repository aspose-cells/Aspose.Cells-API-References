---
title: Cells.CreateRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Creates a Range object from a range of cells
type: docs
url: /net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Creates a [`Range`](../../range/) object from a range of cells.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftCell | String | Upper left cell name. |
| lowerRightCell | String | Lower right cell name. |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
public void Cells_Method_CreateRange()
{
  Workbook workbook = new Workbook();
  Cells cells = workbook.Worksheets[0].Cells;
  Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
  range.Name = "range";
  cells[0, 0].PutValue(2);
  cells[1, 0].PutValue(3);
  cells[0, 1].Formula = "=MAX(range,5)";
  workbook.CalculateFormula();
  Assert.AreEqual(5, cells[0, 1].IntValue);
}
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Creates a [`Range`](../../range/) object from a range of cells.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range |
| firstColumn | Int32 | First column of this range |
| totalRows | Int32 | Number of rows |
| totalColumns | Int32 | Number of columns |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);
public void Cells_Method_CreateRange()
{
    Workbook workbook = new Workbook();
    workbook = new Workbook(Constants.sourcePath + "insertDelete\\testformual3.xls");
    Cells cells = workbook.Worksheets[0].Cells;
    Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);
    Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);
    rangeDest.CopyValue(rangeSrc);

    checkRangeCopyValue_Formual_001(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyValue.xls");
   workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xls");
    checkRangeCopyValue_Formual_001(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyValue.xlsx");
    workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xlsx");
    checkRangeCopyValue_Formual_001(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyValue.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testRangeCopyValue.xml");
    checkRangeCopyValue_Formual_001(workbook);
    workbook.Save(Constants.destPath + "testRangeCopyValue.xls");
}
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Creates a [`Range`](../../range/) object from an address of the range.

```csharp
public Range CreateRange(string address)
```

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |

### Return Value

A [`Range`](../../range/) object

### Examples

```csharp
// Called: Aspose.Cells.Range r1 = workbook.Worksheets[1].Cells.CreateRange("B2:B3");
public void Cells_Method_CreateRange()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Range r = workbook.Worksheets[0].Cells.CreateRange("B2:B3");
    workbook.Worksheets.Add();
    Aspose.Cells.Range r1 = workbook.Worksheets[1].Cells.CreateRange("B2:B3");
    r1.Copy(r);
    Assert.AreEqual(r1[0,0].Formula, "=A2");

}
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Creates a [`Range`](../../range/) object from rows of cells or columns of cells.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | First row index or first column index, zero based. |
| number | Int32 | Total number of rows or columns, one based. |
| isVertical | Boolean | True - Range created from columns of cells. False - Range created from rows of cells. |

### Return Value

A [`Range`](../../range/) object.

### Examples

```csharp
// Called: cells.CreateRange(0, 0, false);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_CreateRange()
        {
            caseName = "testCreateRange_Exception_007";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.CreateRange(0, 0, false);
            string msg = message + "cells.CreateRange(0, 0, false)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



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
// Called: var dataSheetDataRange = dataSheet.Cells.CreateRange(dataSheet.Cells.FirstCell.Name, dataSheet.Cells.LastCell.Name);
private static void Method_String_(Workbook workbook, List<string> columns)
        {
            var dataSheet = workbook.Worksheets.GetSheetByCodeName("Sheet1");
            for (int i = 0; i < columns.Count; ++i)
            {
                dataSheet.Cells[0, i].Value = columns[i];
                var sampleDataCell = dataSheet.Cells[1, i];
                sampleDataCell.Value = "Sample value";
            }
            var dataSheetDataRange = dataSheet.Cells.CreateRange(dataSheet.Cells.FirstCell.Name, dataSheet.Cells.LastCell.Name);
            dataSheetDataRange.Name = "Data0";
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
// Called: Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(2, 1, 9, 4);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Int32_()
        {
            caseName = "testRangeCopy_Hide_003";
            Workbook wbSrc = new Workbook(Constants.sourcePath + "Copy\\hide_001.xls");
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange(2, 1, 9, 4);
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange(2, 1, 9, 4);

            checkRangeCopy_Hide_003(wbDest);
            wbDest.Save(Constants.destPath + "testRangeCopy.xls");
            wbDest = new Workbook(Constants.destPath + "testRangeCopy.xls");
            checkRangeCopy_Hide_003(wbDest);
            wbDest.Save(Constants.destPath + "testRangeCopy.xlsx");
            wbDest = new Workbook(Constants.destPath + "testRangeCopy.xlsx");
            checkRangeCopy_Hide_003(wbDest);
            wbDest.Save(Constants.destPath + "testRangeCopy.xml", SaveFormat.SpreadsheetML);
            wbDest = new Workbook(Constants.destPath + "testRangeCopy.xml");
            checkRangeCopy_Hide_003(wbDest);
            wbDest.Save(Constants.destPath + "testRangeCopy.xls");
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
// Called: cells.CreateRange("B1").Copy(cells.CreateRange("A1"));
[Test]
        public void Method_String_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells["A1"].SetDynamicArrayFormula("=SEQUENCE(7)", new FormulaParseOptions(), true);
            cells.CreateRange("B1").Copy(cells.CreateRange("A1"));
            wb.RefreshDynamicArrayFormulas(true, new CalculationOptions());
            for (int i = 0; i < 7; i++)
            {
                Assert.AreEqual(i + 1, cells[i, 1].IntValue, "B" + (i + 1));
            }
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
// Called: cells.CreateRange(-1, 1, true);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Method_Boolean_()
        {
            caseName = "testCreateRange_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.CreateRange(-1, 1, true);
            string msg = message + "cells.CreateRange(-1, 1, true)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



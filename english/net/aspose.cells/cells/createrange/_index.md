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
// Called: Aspose.Cells.Range range2 = cells.CreateRange(&amp;quot;A28&amp;quot;, &amp;quot;I48&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestCopyShapes_001.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range1 = cells.CreateRange(&quot;A7&quot;, &quot;I27&quot;);
            cells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range range2 = cells.CreateRange(&quot;A28&quot;, &quot;I48&quot;);
            range2.Copy(range1);
            //workbook.Worksheets[1].Copy(workbook.Worksheets[0]);
            Assert.AreEqual(workbook.Worksheets[0].Charts.Count, workbook.Worksheets[1].Charts.Count);
            workbook.Save(Constants.destPath +&quot;TestCopyShapes_001.xls&quot;);
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
// Called: Aspose.Cells.Range srcRange = wbSource.Worksheets[0].Cells.CreateRange(0, 0, 3, 3);
[Test]
        public void Method_Int32_()
        {
            Workbook wbSource = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42699.xlsx&quot;);
            Workbook wbDest = new Workbook();
            wbDest.Worksheets.Add(&quot;COPY VALUES_AND_NUMBER_FORMATS&quot;);
            wbDest.Worksheets.Add(&quot;COPY FORMATS&quot;);
            wbDest.Worksheets.Add(&quot;COPY VALUES&quot;);

            Aspose.Cells.Range srcRange = wbSource.Worksheets[0].Cells.CreateRange(0, 0, 3, 3);
            Aspose.Cells.Range destRangeVNF = wbDest.Worksheets[&quot;COPY VALUES_AND_NUMBER_FORMATS&quot;].Cells.CreateRange(0, 0, 3, 3);
            Aspose.Cells.Range destRangeF = wbDest.Worksheets[&quot;COPY FORMATS&quot;].Cells.CreateRange(0, 0, 3, 3);
            Aspose.Cells.Range destRangeV = wbDest.Worksheets[&quot;COPY VALUES&quot;].Cells.CreateRange(0, 0, 3, 3);

            PasteOptions pasteValuesNFormats = new PasteOptions();
            pasteValuesNFormats.PasteType = (PasteType.ValuesAndNumberFormats);
            destRangeVNF.Copy(srcRange, pasteValuesNFormats);
            Assert.AreEqual(1, destRangeVNF[0, 0].IntValue);

            PasteOptions pasteFormats = new PasteOptions();
            pasteFormats.PasteType = (PasteType.Formats);
            destRangeF.Copy(srcRange, pasteFormats);

            PasteOptions pasteValues = new PasteOptions();
            pasteValues.PasteType = (PasteType.Values);
            destRangeV.Copy(srcRange, pasteValues);

            Util.ReSave(wbDest, SaveFormat.Xlsx);
            //wbDest.Save(Constants.destPath+ &quot;CELLSJAVA42699.xlsx&quot;);
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
// Called: Aspose.Cells.Range sourceRange = selectedWorksheet.Cells.CreateRange(&amp;quot;A1:I12&amp;quot;);
[Test]
        public void Method_String_()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45948/&quot;;

            Workbook workbook = new Workbook(filePath + &quot;a.xlsx&quot;);
            Worksheet selectedWorksheet = workbook.Worksheets[&quot;Sheet1&quot;];

            //Create Range
            Aspose.Cells.Range sourceRange = selectedWorksheet.Cells.CreateRange(&quot;A1:I12&quot;);

            Workbook targetWorkbook = new Workbook(FileFormatType.Xlsx);
            WorksheetCollection targetWsc = targetWorkbook.Worksheets;
            Worksheet targetWs = targetWsc[0];
            Aspose.Cells.Range targetRange = targetWs.Cells.CreateRange(0, 0, sourceRange.RowCount, sourceRange.ColumnCount);

            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            targetRange.Copy(sourceRange, options);
            targetWorkbook.Save(CreateFolder(filePath) + &quot;out.html&quot;, SaveFormat.Html);
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
// Called: Aspose.Cells.Range range = cells.CreateRange(0, 1, false);
[Test, Category(&quot;Bug&quot;)]
        public void Method_Boolean_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange(0, 1, false);
            range.Name = &quot;myRow&quot;;
            workbook.Save(Constants.destPath + &quot;TestNamedColumn.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;TestNamedColumn.xml&quot;);
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



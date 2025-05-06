---
title: Cells.ImportCSV
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Import a CSV file to the cells
type: docs
url: /net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

Import a CSV file to the cells.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| splitter | String | The splitter |
| convertNumericData | Boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### Examples

```csharp
// Called: cells.ImportCSV(Constants.sourcePath + &amp;quot;CSV File 76 Mb.csv&amp;quot;, &amp;quot;;&amp;quot;, true, 0, 0);
[Test, Category(&quot;Bug&quot;)]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.ImportCSV(Constants.sourcePath + &quot;CSV File 76 Mb.csv&quot;, &quot;;&quot;, true, 0, 0);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

Import a CSV file to the cells.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The CSV file stream. |
| splitter | String | The splitter |
| convertNumericData | Boolean | Whether the string in text file is converted to numeric data. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

Import a CSV file to the cells.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The CSV file name. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### Examples

```csharp
// Called: cells.ImportCSV(Constants.sourcePath + &amp;quot;SWDATAbe2359e70a22dc8c0218da0f66b228da_1553673199564.csv&amp;quot;, options, 0, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET46574.Xlsx&quot;);
            string s = workbook.Worksheets[0].Name;
            Cells cells = workbook.Worksheets[0].Cells;
            TxtLoadOptions options = new TxtLoadOptions();
            options.SeparatorString = (&quot;~&quot;);
            options.LoadStyleStrategy = (TxtLoadStyleStrategy.ExactFormat);
            options.HasFormula = (true);
            cells.ImportCSV(Constants.sourcePath + &quot;SWDATAbe2359e70a22dc8c0218da0f66b228da_1553673199564.csv&quot;, options, 0, 1);
            Assert.AreEqual(s, &quot;Qatama Rates&quot;);
            workbook.Save(Constants.destPath + &quot;CellsJava42862.xlsb&quot;);
        }
```

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

Import a CSV file to the cells.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The CSV file stream. |
| options | TxtLoadOptions | The load options for reading text file |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



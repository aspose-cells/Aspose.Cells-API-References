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
// Called: cells.ImportCSV(Constants.sourcePath + "CELLSJAVA40883.csv", ",", true, 0, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("sf");
            cells.ImportCSV(Constants.sourcePath + "CELLSJAVA40883.csv", ",", true, 0, 0);
            Assert.AreEqual(cells["A2"].GetStyle().IsDateTime, true);
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
// Called: sheet.Cells.ImportCSV(filePath + "winemag-data_first150k.csv", opts, 0, 0);
public Workbook Method_Int32_(string filePath, Workbook excelTemplate)
        {
            TxtLoadOptions opts = new TxtLoadOptions();
            opts.Separator = ',';
            opts.ConvertDateTimeData = true;
            opts.ConvertNumericData = true;
            opts.ParsingFormulaOnOpen = true;

            Console.WriteLine(String.Format("Started writing Data of : %s into sheet : %s", "winemag-data_first150k.csv", "Sheet1"));

            Workbook dataWorkbook = new Workbook(filePath + "winemag-data_first150k.csv", opts);
            Worksheet sheet = dataWorkbook.Worksheets[0];
            sheet.Cells.ImportCSV(filePath + "winemag-data_first150k.csv", opts, 0, 0);

            excelTemplate.Worksheets["Sheet1"].Copy(sheet);
            excelTemplate.Worksheets["Sheet1"].IsVisible = false;

            Console.WriteLine(String.Format("Finished writing Data into sheet : %s", "Sheet1"));

            return excelTemplate;
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



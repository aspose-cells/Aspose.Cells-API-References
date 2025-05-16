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
// Called: cells.ImportCSV(Constants.sourcePath + "example.csv", ";", true, 0, 0);
[Test, Category("Bug")]
        public void Cells_Method_ImportCSV()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.ImportCSV(Constants.sourcePath + "example.csv", ";", true, 0, 0);
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

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare CSV data stream
            string csvData = "Name,Age\nJohn,30\nJane,25";
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)))
            {
                try
                {
                    // Call ImportCSV with parameters: (Stream, ",", true, 0, 0)
                    worksheet.Cells.ImportCSV(stream, ",", true, 0, 0);

                    Console.WriteLine("CSV data imported successfully to cells A1:B3");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error executing ImportCSV method: {ex.Message}");
                }
            }

            // Save the result
            workbook.Save("CellsMethodImportCSVWithStreamDemo.xlsx");
        }
    }
}
```

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
// Called: sheet.Cells.ImportCSV(filePath + "example.csv", opts, 0, 0);
public Workbook Cells_Method_ImportCSV(string filePath, Workbook excelTemplate)
        {
            TxtLoadOptions opts = new TxtLoadOptions();
            opts.Separator = ',';
            opts.ConvertDateTimeData = true;
            opts.ConvertNumericData = true;
            opts.ParsingFormulaOnOpen = true;

            Console.WriteLine(String.Format("Started writing Data of : %s into sheet : %s", "example.csv", "Sheet1"));

            Workbook dataWorkbook = new Workbook(filePath + "example.csv", opts);
            Worksheet sheet = dataWorkbook.Worksheets[0];
            sheet.Cells.ImportCSV(filePath + "example.csv", opts, 0, 0);

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

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create CSV data stream
            string csvData = "Name,Age\nJohn,30\nAlice,25";
            using (MemoryStream stream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)))
            {
                // Create TXT load options with comma separator
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';

                try
                {
                    // Import CSV from stream starting at cell A1 (row 0, column 0)
                    worksheet.Cells.ImportCSV(stream, loadOptions, 0, 0);

                    Console.WriteLine("CSV imported successfully to A1:B3");
                    Console.WriteLine($"Cell B1 value: {worksheet.Cells["B1"].StringValue}");
                    Console.WriteLine($"Cell B2 value: {worksheet.Cells["B2"].StringValue}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error importing CSV: {ex.Message}");
                }
            }

            // Save the result
            workbook.Save("ImportCSVFromStreamDemo.xlsx");
        }
    }
}
```

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



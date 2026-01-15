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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Path to the CSV file
            string csvPath = "example.csv";
            
            // Import CSV data starting at cell A1 (row 0, column 0)
            // Using semicolon as delimiter and converting numeric data
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Save the workbook
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
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
namespace AsposeCellsExamples
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
            Cells cells = worksheet.Cells;

            // Create sample CSV data in memory
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Call ImportCSV method with Stream, String, Boolean, Int32, Int32 parameters
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Save the workbook
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create CSV load options
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Sample CSV file path (replace with actual path in your environment)
            string csvFilePath = "example.csv";
            
            // Import CSV data starting at cell A1 (row 0, column 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Save the workbook
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
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
namespace AsposeCellsExamples
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

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the Cells collection
            Cells cells = worksheet.Cells;

            // Create sample CSV data
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // Create a memory stream with the CSV data
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // Create TxtLoadOptions for CSV import
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // Import CSV data starting at row 0, column 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Save the workbook
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Dispose the stream
                csvStream.Dispose();
            }
        }
    }
}
```

### See Also

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



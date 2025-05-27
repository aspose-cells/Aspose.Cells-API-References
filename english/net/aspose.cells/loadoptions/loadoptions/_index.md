---
title: LoadOptions.LoadOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public LoadOptions()
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Create LoadOptions using constructor with LoadFormat
            LoadOptions options = new LoadOptions(LoadFormat.Excel97To2003);
            
            // Set properties
            options.CheckDataValid = true;
            
            // Load workbook with options
            Workbook workbook = new Workbook("example.xls", options);
            
            // Save to PDF
            workbook.Save("example.pdf");
        }
    }
}
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Create sample CSV content
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Create LoadOptions with LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Load CSV file with created options
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Demonstrate successful load by reading cell
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Save as XLSX to show conversion capability
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### See Also

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



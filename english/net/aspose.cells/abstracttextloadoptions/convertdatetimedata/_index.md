---
title: AbstractTextLoadOptions.ConvertDateTimeData
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true
type: docs
url: /net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Gets or sets a value that indicates whether the string in text file is converted to date data. Default value is true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Create CSV data with a date string
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Create text load options with ConvertDateTimeData set to false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Load the CSV data
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Output the values (should remain as strings)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Now load with ConvertDateTimeData set to true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Output the converted values
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



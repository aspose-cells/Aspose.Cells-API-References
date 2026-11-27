---
title: "AbstractTextLoadOptions.ConvertDateTimeData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractTextLoadOptions-egenskap. Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/abstracttextloadoptions/convertdatetimedata/
---
## AbstractTextLoadOptions.ConvertDateTimeData property

Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.

```csharp
public bool ConvertDateTimeData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertDateTimeDataDemo
    {
        public static void Run()
        {
            // Skapa CSV-data med en datumsträng
            string csvData = "\"2023-05-15\",\"123.45\"";

            // Skapa textinläsningsalternativ med ConvertDateTimeData satt till false
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            options.ConvertDateTimeData = false;
            options.ConvertNumericData = false;

            // Läs in CSV-data
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Skriv ut värdena (bör förbli som strängar)
            Console.WriteLine("Cell A1 value: " + worksheet.Cells[0, 0].StringValue); // Outputs "2023-05-15" as string
            Console.WriteLine("Cell B1 value: " + worksheet.Cells[0, 1].StringValue); // Outputs "123.45" as string

            // Läs nu in med ConvertDateTimeData satt till true
            options.ConvertDateTimeData = true;
            options.ConvertNumericData = true;
            workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            worksheet = workbook.Worksheets[0];

            // Skriv ut de konverterade värdena
            Console.WriteLine("Cell A1 value (converted): " + worksheet.Cells[0, 0].DateTimeValue); // Outputs DateTime
            Console.WriteLine("Cell B1 value (converted): " + worksheet.Cells[0, 1].DoubleValue);  // Outputs 123.45 as double
        }
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "AbstractTextLoadOptions.ConvertNumericData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractTextLoadOptions‑egenskap. Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/abstracttextloadoptions/convertnumericdata/
---
## AbstractTextLoadOptions.ConvertNumericData property

Hämtar eller anger ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.

```csharp
public bool ConvertNumericData { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Skapa exempel‑CSV‑data med numeriska och textvärden
            string csvData = "ID,Name,Price,Quantity\n" +
                            "1,Product A,19.99,5\n" +
                            "2,Product B,\"24.50\",\"10\"\n" +
                            "3,Product C,15.75,\"N/A\"";

            // Skapa TxtLoadOptions med ConvertNumericData satt till true
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertNumericData = true,
                ConvertDateTimeData = true
            };

            // Läs in CSV-data i en arbetsbok
            Workbook workbook = new Workbook(new System.IO.MemoryStream(Encoding.UTF8.GetBytes(csvData)), options);
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa numerisk konvertering
            Console.WriteLine("Cell B2 (Product A Price) value type: " + worksheet.Cells["B2"].Value.GetType());
            Console.WriteLine("Cell B2 value: " + worksheet.Cells["B2"].Value);

            // Visa textvärden som inte kunde konverteras
            Console.WriteLine("\nCell D4 (N/A) value type: " + worksheet.Cells["D4"].Value.GetType());
            Console.WriteLine("Cell D4 value: " + worksheet.Cells["D4"].Value);

            // Visa hur citerade tal fortfarande konverteras när ConvertNumericData är true
            Console.WriteLine("\nCell C3 (Quoted \"24.50\") value type: " + worksheet.Cells["C3"].Value.GetType());
            Console.WriteLine("Cell C3 value: " + worksheet.Cells["C3"].Value);
        }
    }
}
```

### Se även

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



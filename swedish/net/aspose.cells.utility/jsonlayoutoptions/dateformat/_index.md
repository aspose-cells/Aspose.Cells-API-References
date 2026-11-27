---
title: "JsonLayoutOptions.DateFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions-egenskap. Hämtar och anger formatet för datumvärdet"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Hämtar och anger formatet för datumvärdet.

```csharp
public string DateFormat { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Konfigurera JSON-importalternativ med anpassat datumformat
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // Importera JSON-data med datumvärden
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // Verifiera att datumet importerades med korrekt formatering
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



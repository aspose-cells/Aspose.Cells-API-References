---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportRangeToJsonOptions-egenskap. Anger om intervallet innehåller en rubrikrad"
type: docs
url: /sv/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Anger om intervallet innehåller en rubrikrad.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata med rubriker
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa intervall att exportera
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Skapa en ExportRangeToJsonOptions-instans
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Visa aktuellt HasHeaderRow-värde (standard är falskt)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // Ställ in HasHeaderRow till true
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportera till JSON med rubriker
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Ställ in HasHeaderRow till false
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exportera till JSON utan rubriker
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Spara arbetsboken
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



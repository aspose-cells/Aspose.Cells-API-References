---
title: "ExportRangeToJsonOptions.Indent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportRangeToJsonOptions-egenskap. Anger indraget"
type: docs
url: /sv/net/aspose.cells.utility/exportrangetojsonoptions/indent/
---
## ExportRangeToJsonOptions.Indent property

Indikerar indraget.

```csharp
public string Indent { get; set; }
```

### Anmärkningar

Om indraget är null eller tomt, formateras inte den exporterade JSON‑filen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Skapa en ExportRangeToJsonOptions-instans
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Visa aktuellt indrag (standard är null)
            Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));

            // Exportera med standardindrag (kompakt JSON)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
            string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);

            // Ställ in indrag till 4 mellanslag
            options.Indent = "    ";
            string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);

            // Ställ in indrag till tabbtecken
            options.Indent = "\t";
            string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
        }
    }
}
```

### Se även

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



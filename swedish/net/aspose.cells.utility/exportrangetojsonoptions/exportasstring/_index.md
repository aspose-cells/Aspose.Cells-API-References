---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportRangeToJsonOptions-egenskap. Exporterar cellernas strängvärde till json"
type: docs
url: /sv/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Exporterar cellernas strängvärde till JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i celler med olika datatyper
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // Skapa en ExportRangeToJsonOptions-instans
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Visa aktuellt ExportAsString‑värde
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Exportera utan ExportAsString (standardbeteende)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // Ställ in ExportAsString till true
            options.ExportAsString = true;

            // Exportera med ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Spara arbetsboken
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)



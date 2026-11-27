---
title: "DbfSaveOptions.ExportAsString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DbfSaveOptions-egenskap. Anger om export sker som strängvärde"
type: docs
url: /sv/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Indikerar om export som strängvärde

```csharp
public bool ExportAsString { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med blandade typer
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Skapa en DbfSaveOptions-instans
            DbfSaveOptions options = new DbfSaveOptions();

            // Visa aktuellt ExportAsString‑värde
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Ställ in ExportAsString till true (alla värden kommer att exporteras som strängar)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Spara med ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Ställ in ExportAsString till false (värdena behåller sina ursprungliga typer)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Spara med ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Se även

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)



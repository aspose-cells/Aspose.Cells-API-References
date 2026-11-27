---
title: "Protection.AllowDeletingRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Protection-egenskap. Representerar om rader får tas bort i ett skyddat kalkylblad"
type: docs
url: /sv/net/aspose.cells/protection/allowdeletingrow/
---
## Protection.AllowDeletingRow property

Representerar om radering av rader är tillåten på ett skyddat kalkylblad.

```csharp
public bool AllowDeletingRow { get; set; }
```

### Anmärkningar

Raderna som innehåller cellerna som ska tas bort måste vara olåsta när bladet är skyddat, och alternativet "Select unlocked cells" måste vara aktiverat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowDeletingRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in skyddsinställningar
            Protection protection = sheet.Protection;
            protection.AllowDeletingRow = true;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingColumn = true;

            // Skydda kalkylbladet
            sheet.Protect(ProtectionType.All);

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Läs in den sparade arbetsboken för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];

            // Verifiera AllowDeletingRow och andra egenskaper
            Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
            Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
            Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
            Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
        }
    }
}
```

### Se även

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



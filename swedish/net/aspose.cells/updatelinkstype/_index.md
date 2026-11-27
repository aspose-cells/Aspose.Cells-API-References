---
title: "Enum UpdateLinksType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.UpdateLinksType enum. Representerar hur länkar till andra arbetsböcker uppdateras när arbetsboken öppnas"
type: docs
url: /sv/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Representerar hur länkar till andra arbetsböcker uppdateras när arbetsboken öppnas.

```csharp
public enum UpdateLinksType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| UserSet | `0` | Be användaren att uppdatera. |
| Never | `1` | Uppdatera inte, och be inte användaren. |
| Always | `2` | Uppdatera alltid. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt arbetsbokens inställningar
            WorkbookSettings settings = workbook.Settings;

            // Ställ in UpdateLinksType till Alltid uppdatera
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Spara arbetsboken
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Skriv ut den aktuella UpdateLinksType-inställningen
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



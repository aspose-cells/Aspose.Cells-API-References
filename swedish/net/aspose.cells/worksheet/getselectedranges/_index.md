---
title: "Worksheet.GetSelectedRanges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Hämtar valda cellområden i designerns kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Hämtar markerade cellområden i designerns kalkylblad.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Returvärde

En ArrayList som innehåller markerade områden.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd i stället metoden Worksheet.GetSelectedAreas(). Denna egenskap kommer att tas bort 12 månader senare från och med mars 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Obs: GetSelectedRanges är markerad som föråldrad i reflektionen
                // Detta demonstrerar metodanropet enligt begäran
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Visa antalet markerade områden
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Visa varje markerat område
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Spara arbetsboken
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



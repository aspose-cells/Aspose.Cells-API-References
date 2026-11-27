---
title: "Klass DeleteOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DeleteOptions klass. Representerar inställningen för att ta bort rader/kolumner"
type: docs
url: /sv/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Representerar inställningen för att ta bort rader/kolumner.

```csharp
public class DeleteOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Hämtar/anger övervakaren för att spåra ändringar som orsakas av borttagningen. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Visa den ursprungliga datan
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Skapa DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Ta bort den andra raden (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Visa datan efter borttagning
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Spara arbetsboken
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



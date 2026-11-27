---
title: "Range.ClearHyperlinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Tar bara bort hyperlänkar"
type: docs
url: /sv/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Tar bara bort hyperlänkar.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| clearFormat | Boolean | Anger om formatet för hyperlänkar ska rensas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett range och lägg till några hyperlänkar för demonstration
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Rensa hyperlänkar med formatbevarande (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Lägg till hyperlänkar igen
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Rensa hyperlänkar utan formatbevarande (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Spara arbetsboken
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



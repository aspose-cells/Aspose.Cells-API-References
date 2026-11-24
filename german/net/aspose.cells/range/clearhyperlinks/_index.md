---
title: "Range.ClearHyperlinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Entfernt nur Hyperlinks"
type: docs
url: /de/net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Entfernt nur Hyperlinks.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| clearFormat | Boolean | Gibt an, ob das Format von Hyperlinks gelöscht werden soll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Bereich und füge einige Hyperlinks zur Demonstration hinzu
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Hyperlinks mit Formatbeibehaltung löschen (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Hyperlinks erneut hinzufügen
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Hyperlinks ohne Formatbeibehaltung löschen (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



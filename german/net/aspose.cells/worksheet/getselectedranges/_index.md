---
title: "Worksheet.GetSelectedRanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Ruft die ausgewählten Zellbereiche im Designer-Tabellenblatt ab"
type: docs
url: /de/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Liest die ausgewählten Zellbereiche im Designer-Tabellenblatt.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Rückgabewert

Eine ArrayList, die ausgewählte Bereiche enthält.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.GetSelectedAreas(). Diese Eigenschaft wird 12 Monate später, seit März 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben könnten.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Hinweis: GetSelectedRanges ist in der Reflexion als veraltet markiert.
                // Dies demonstriert den Methodenaufruf wie angefordert.
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Zeige die Anzahl der ausgewählten Bereiche an.
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Zeige jeden ausgewählten Bereich an.
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



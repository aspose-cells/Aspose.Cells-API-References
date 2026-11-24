---
title: "Font.Equals"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Methode. Prüft, ob zwei Schriften gleich sind"
type: docs
url: /de/net/aspose.cells/font/equals/
---
## Font.Equals method

Prüft, ob zwei Schriftarten gleich sind.

```csharp
public bool Equals(Font font)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Schriftart | Schriftart | Verglichenes Schriftobjekt. |

### Rückgabewert

Wahr, wenn es dem verglichenen Schriftobjekt entspricht.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie zwei Schriftobjekte zum Vergleich
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Rufen Sie die Equals-Methode auf, um die Schriften zu vergleichen
                bool areEqual = font1.Equals(font2);

                // Ergebnis anzeigen
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Ändern Sie eine Schrift, damit sie sich unterscheidet
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



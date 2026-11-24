---
title: "Enum ColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ColorType Enum. Stellt alle Farbtypen dar"
type: docs
url: /de/net/aspose.cells/colortype/
---
## ColorType enumeration

Stellt alle Farbtypen dar

```csharp
public enum ColorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Automatische Farbe. |
| AutomaticIndex | `1` | Es ist eine automatische Farbe, aber die angezeigte Farbe hängt von den Einstellungen des Betriebssystems ab. |
| RGB | `2` | Die RGB-Farbe. |
| IndexedColor | `3` | Der Farbindex in der Farbpalette. |
| Theme | `4` | Die Themenfarbe. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellt ein neues Arbeitsbuch für die Demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstriere die Verwendung von ColorType-Enum-Werten
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Die Enum-Werte anzeigen
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Erstelle eine Zelle und setze ihren Wert
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Erstelle einen Stil und wende ihn auf die Zelle an
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Speichere die Arbeitsmappe
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



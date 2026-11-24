---
title: "Cell.SetCharacters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzt das Rich-Text-Format der Zelle"
type: docs
url: /de/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Setzt das Rich-Text-Format der Zelle.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeichen | FontSetting[] | Alle Zeichen-Objekte. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Setze den Zellenwert, um Rich-Text-Formatierung anzuwenden
            cell.Value = "Hello World!";

            try
            {
                // Erstelle Schriftarteinstellungen für verschiedene Teile des Textes
                FontSetting[] fontSettings = new FontSetting[2];

                // Formatiere die ersten 5 Zeichen (Hello) als fett rot
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Formatiere die restlichen Zeichen ( World!) als kursiv blau
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Wende die formatierten Zeichen-Einstellungen mit SetCharacters an
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



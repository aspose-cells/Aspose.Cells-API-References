---
title: "Cell.GetCharacters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt alle Characters-Objekte zurück, die einen Bereich von Zeichen im Zellentext darstellen."
type: docs
url: /de/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Gibt alle Characters‑Objekte zurück, die einen Zeichenbereich innerhalb des Zellentextes darstellen.

```csharp
public FontSetting[] GetCharacters()
```

### Rückgabewert

Alle Characters-Objekte

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setzen Sie HTML-formatierten Text in Zelle A1 mit unterschiedlichen Formatierungsteilen
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Rufen Sie die Zeichenformatierungsinformationen aus Zelle A1 ab
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Geben Sie die Formatierungsinformationen aus
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Gibt alle Characters‑Objekte zurück, die einen Zeichenbereich innerhalb des Zellentextes darstellen.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Flag | Boolean | Gibt an, ob ein Tabellenstil auf die Zelle angewendet wird, wenn sich die Zelle in einer Tabelle befindet. |

### Rückgabewert

Alle Characters-Objekte

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Text zu Zelle C8 mit Formatierung hinzu
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Formatieren Sie Teile des Textes
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Rufen Sie alle Schriftarteinstellungen mit Formatierung ab
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Schriftfarben anzeigen
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Siehe auch

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



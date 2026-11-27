---
title: "Cell.GetCharacters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Returnerar alla Characters‑objekt som representerar ett teckenintervall inom cellens text"
type: docs
url: /sv/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Returnerar alla Characters-objekt som representerar ett teckenintervall inom cellens text.

```csharp
public FontSetting[] GetCharacters()
```

### Returvärde

Alla Characters‑objekt

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange HTML‑formaterad text i cell A1 med olika formateringsdelar
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Hämta teckenformateringsinformationen från cell A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Skriv ut formateringsinformationen
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

### Se även

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Returnerar alla Characters-objekt som representerar ett teckenintervall inom cellens text.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| flagga | Boolean | Anger om tabellstil ska tillämpas på cellen om cellen är i tabellen. |

### Returvärde

Alla Characters‑objekt

### Exempel

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
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till text i cell C8 med formatering
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Formatera delar av texten
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Hämta alla teckensnittinställningar med formatering
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Visa teckensnittsfärger
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Se även

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



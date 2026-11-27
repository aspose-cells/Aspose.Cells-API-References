---
title: "Shape.GetCharacters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Returnerar alla Characters‑objekt som representerar ett teckenintervall inom texten."
type: docs
url: /sv/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Returnerar alla Characters-objekt som representerar ett teckenintervall inom texten.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Returvärde

Alla Characters‑objekt

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Shape.GetRichFormattings()‑metoden. Denna metod kommer att tas bort 12 månader senare, från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textrutaform till kalkylbladet med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Hämta tecknen från formen
            ArrayList characters = shape.GetCharacters();

            // Visa information om varje tecken
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



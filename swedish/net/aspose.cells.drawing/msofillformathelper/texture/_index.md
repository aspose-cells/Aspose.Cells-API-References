---
title: "MsoFillFormatHelper.Texture"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper-egenskap. Hämtar texturfyllningstypen"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Hämtar typen av texturfyllning.

```csharp
public TextureType Texture { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion (ingen publik konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visa det aktuella värdet för Texture-egenskapen (skrivskyddad)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Demonstrera att egenskapen är skrivskyddad genom att försöka sätta den (kommenterad)
                // fillHelper.Texture = TextureType.Canvas; // Detta skulle orsaka ett kompileringsfel

                // Visa alla tillgängliga texturtyper som referens
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



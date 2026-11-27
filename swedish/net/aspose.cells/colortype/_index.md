---
title: "Enum ColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ColorType enum. Representerar alla färgtyper"
type: docs
url: /sv/net/aspose.cells/colortype/
---
## ColorType enumeration

Representerar alla färgtyper

```csharp
public enum ColorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | Automatisk färg. |
| AutomaticIndex | `1` | Det är en automatisk färg, men den visade färgen beror på inställningarna i operativsystemet. |
| RGB | `2` | RGB-färgen. |
| IndexedColor | `3` | Färgens index i färgpaletten. |
| Theme | `4` | Temafärgen. |

### Exempel

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
                // Skapa en ny arbetsbok för demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrera användning av ColorType enum‑värden
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Visa enum‑värden
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Skapa en cell och sätt dess värde
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Skapa en stil och tillämpa den på cellen
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



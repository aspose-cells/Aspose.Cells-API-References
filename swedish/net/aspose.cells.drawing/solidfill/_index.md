---
title: "Klass SolidFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.SolidFill-klass. Inkapslar objektet som representerar format för solid fyllning"
type: docs
url: /sv/net/aspose.cells.drawing/solidfill/
---
## SolidFill class

Inkapslar objektet som representerar solid fyllningsformat

```csharp
public class SolidFill : Fill
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/solidfill/cellscolor/) { get; set; } | Hämtar och anger [`CellsColor`](./cellscolor/) objektet. |
| [Color](../../aspose.cells.drawing/solidfill/color/) { get; set; } | Hämtar eller anger färgen. |
| [Transparency](../../aspose.cells.drawing/solidfill/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/solidfill/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/solidfill/gethashcode/)() | Hämtar hash‑koden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.Drawing;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;

    public class DrawingClassSolidFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en enkel rektangelform på bladet
                Shape rect = sheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);

                // Konfigurera formen för att använda en solid fyllning
                rect.Fill.FillType = FillType.Solid;

                // Hämta SolidFill-objektet
                SolidFill solidFill = rect.Fill.SolidFill;

                // Ange egenskaper för solid fyllning
                solidFill.Color = Color.CornflowerBlue;   // System.Drawing.Color
                solidFill.Transparency = 0.25;            // 0 = opaque, 1 = fully transparent

                // Åtkomst till CellsColor-egenskapen (läsa/skriva)
                CellsColor cellsColor = solidFill.CellsColor;
                if (cellsColor != null)
                {
                    Console.WriteLine("CellsColor object is available.");
                }
                else
                {
                    Console.WriteLine("CellsColor is null (default).");
                }

                Console.WriteLine($"SolidFill created with Color={solidFill.Color.Name}, Transparency={solidFill.Transparency}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SolidFill: {ex.Message}");
            }

            // Spara arbetsboken för att verifiera formens utseende
            workbook.Save("DrawingClassSolidFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



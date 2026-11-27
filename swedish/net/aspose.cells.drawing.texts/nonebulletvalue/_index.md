---
title: "Klass NoneBulletValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue‑klass. Representerar ingen punktlista"
type: docs
url: /sv/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Representerar ingen punkt.

```csharp
public class NoneBulletValue : BulletValue
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Hämtar typen av punktlistans värde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till text i en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Skapa en TextBox för att tillämpa punktlistinställningar
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Skapa en instans av NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Kontrollera typen av punktlista (bör vara None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Spara arbetsboken för att demonstrera ändringarna
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Se även

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



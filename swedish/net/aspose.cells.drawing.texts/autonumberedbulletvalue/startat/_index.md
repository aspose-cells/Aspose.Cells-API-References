---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoNumberedBulletValue-egenskap. Hämtar och anger startnumret för bulleten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Hämtar och anger startnumret för punkten.

```csharp
public int StartAt { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Skapa en AutoNumberedBulletValue-instans
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Visa det aktuella StartAt-värdet
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // Ändra StartAt-värdet
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Skapa en form för att demonstrera bulleten i sammanhanget
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Applicera bullet-stilen (obs: den faktiska tillämpningsmetoden visas inte i reflektionen)
                // För demonstration sparar vi bara arbetsboken
                workbook.Save("StartAtPropertyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

}
```

### Se även

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



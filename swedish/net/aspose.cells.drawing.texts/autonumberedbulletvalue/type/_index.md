---
title: "AutoNumberedBulletValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoNumberedBulletValue-egenskap. Hämtar bulletens typ"
type: docs
url: /sv/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Hämtar typen av punkten.

```csharp
public override BulletType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att lägga till text med bullets
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Skapa ett auto-numrerat bulletvärde
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Eftersom vi inte kan sätta BulletValue direkt måste vi hitta ett annat sätt
            // för att applicera bullet-stilen. Detta kan innebära att använda formens textformatering
            // eller andra tillgängliga metoder i API:et.
            // För demonstration visar vi bara bullet-typen
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Lägg till text i paragrafen via formens textkropp
            shape.TextBody.Text = "First Item";

            // Lägg till en annan paragraf med ett annat numreringsschema
            // Eftersom vi inte kan lägga till, använder vi nästa tillgängliga stycke
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Visa bullet-typen (skrivskyddad egenskap)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Lägg till text till det andra stycket
            shape.TextBody.Text += "\nSecond Item";

            // Spara arbetsboken för att demonstrera bullet‑effekterna
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Se även

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



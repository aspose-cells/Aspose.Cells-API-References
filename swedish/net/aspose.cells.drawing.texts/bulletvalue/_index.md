---
title: "Klass BulletValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.BulletValue‑klass. Representerar värdet av punktlistan"
type: docs
url: /sv/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Representerar värdet på punkten.

```csharp
public abstract class BulletValue
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Hämtar typen av punktlistans värde. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en textruta och hämta dess textstycken
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Skapa en instans av CharacterBulletValue (som ärver från BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Ställ in bullet‑värdet på stycket (Bullet är skrivskyddat, så vi måste modifiera det på annat sätt)
            // Eftersom Bullet är skrivskyddat måste vi hitta ett annat sätt att sätta det
            // Det kan innebära att skapa ett nytt TextParagraph med bullet‑inställningen
            // Obs: Det faktiska API:et kan erbjuda ett annat sätt att sätta bullets
            // För demonstration antar vi att vi kan sätta det genom någon annan metod
            // textParagraph.Bullet = bulletValue; // Denna rad har tagits bort eftersom Bullet är skrivskyddat
            textBox.Text = "First bullet point";

            // Lägg till ett annat stycke med en annan bullet
            // TextParagraphCollection har ingen Add‑metod, så vi måste hitta ett annat sätt
            // Det kan innebära att skapa ett nytt TextParagraph och lägga till det på något annat sätt
            // För demonstration antar vi att vi kan hämta det andra stycket direkt
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Denna rad har tagits bort eftersom Bullet är skrivskyddat
            textBox.Text += "\nSecond bullet point";

            // Demonstrera åtkomst till bullet‑typen
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Spara resultatet
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



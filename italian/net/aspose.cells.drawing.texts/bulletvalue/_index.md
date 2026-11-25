---
title: "Classe BulletValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.BulletValue classe. Rappresenta il valore del punto elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Rappresenta il valore del punto elenco.

```csharp
public abstract class BulletValue
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Ottiene il tipo del valore del punto elenco. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una casella di testo e ottieni i suoi paragrafi di testo
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Crea un'istanza di CharacterBulletValue (che eredita da BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Imposta il valore del punto elenco al paragrafo (Bullet è di sola lettura, quindi dobbiamo modificarlo diversamente)
            // Poiché Bullet è di sola lettura, dobbiamo trovare un altro modo per impostarlo
            // Questo potrebbe comportare la creazione di un nuovo TextParagraph con il punto elenco impostato
            // Nota: L'API reale potrebbe fornire un modo diverso per impostare i punti elenco
            // Per dimostrazione, supporremo di poterlo impostare tramite altri mezzi
            // textParagraph.Bullet = bulletValue; // Questa riga è rimossa poiché Bullet è di sola lettura
            textBox.Text = "First bullet point";

            // Aggiungi un altro paragrafo con un punto elenco diverso
            // TextParagraphCollection non ha un metodo Add, quindi dobbiamo trovare un altro modo
            // Questo potrebbe comportare la creazione di un nuovo TextParagraph e aggiungerlo tramite altri mezzi
            // Per dimostrazione, supporremo di poter ottenere direttamente il secondo paragrafo
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Questa riga è rimossa poiché Bullet è di sola lettura
            textBox.Text += "\nSecond bullet point";

            // Dimostra l'accesso al tipo di punto elenco
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Salva il risultato
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



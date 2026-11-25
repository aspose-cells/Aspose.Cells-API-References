---
title: "AutoNumberedBulletValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoNumberedBulletValue. Ottiene il tipo del punto elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Ottiene il tipo del punto elenco.

```csharp
public override BulletType Type { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per aggiungere testo con punti elenco
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Crea un valore di punto elenco numerato automaticamente
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Poiché non possiamo impostare direttamente BulletValue, dovremo trovare un altro modo
            // per applicare lo stile del punto elenco. Questo potrebbe richiedere l'uso della formattazione del testo della forma
            // oppure altri metodi disponibili nell'API.
            // Per dimostrazione, visualizzeremo semplicemente il tipo di punto elenco
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Aggiungi testo al paragrafo tramite il corpo di testo della forma
            shape.TextBody.Text = "First Item";

            // Aggiungi un altro paragrafo con uno schema di numerazione diverso
            // Poiché non possiamo Add, utilizzeremo il prossimo paragrafo disponibile
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Visualizza il tipo di elenco puntato (proprietà di sola lettura)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Aggiungi testo al secondo paragrafo
            shape.TextBody.Text += "\nSecond Item";

            // Salva la cartella di lavoro per dimostrare gli effetti dell'elenco puntato
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



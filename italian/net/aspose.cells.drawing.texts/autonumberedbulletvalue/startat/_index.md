---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoNumberedBulletValue. Ottiene e imposta il numero iniziale del punto elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Ottiene e imposta il numero iniziale del punto elenco.

```csharp
public int StartAt { get; set; }
```

### Esempi

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
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea un'istanza di AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Visualizza il valore corrente di StartAt
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // Modifica il valore di StartAt
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Crea una forma per dimostrare il punto elenco nel contesto
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Applica lo stile del punto elenco (nota: il metodo di applicazione reale non è mostrato nella riflessione)
                // Per dimostrazione, salveremo semplicemente la cartella di lavoro
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

### Vedi anche

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



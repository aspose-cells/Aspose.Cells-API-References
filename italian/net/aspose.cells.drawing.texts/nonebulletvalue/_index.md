---
title: "Classe NoneBulletValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue classe. Rappresenta nessun punto elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Rappresenta nessun punto elenco.

```csharp
public class NoneBulletValue : BulletValue
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Ottiene il tipo del valore del punto elenco. |

### Esempi

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
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di testo a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Crea un TextBox per applicare le impostazioni del punto elenco
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Crea un'istanza di NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Verifica il tipo del punto elenco (dovrebbe essere None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Salva la cartella di lavoro per dimostrare le modifiche
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



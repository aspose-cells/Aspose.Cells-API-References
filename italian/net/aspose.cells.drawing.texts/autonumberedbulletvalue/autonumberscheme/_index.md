---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoNumberedBulletValue. Rappresenta lo schema del numero automatico"
type: docs
url: /it/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Rappresenta lo schema del numero automatico.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova istanza di AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Visualizza il valore iniziale di AutonumberScheme
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Imposta un nuovo valore di AutonumberScheme
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Crea una cartella di lavoro per dimostrare l'elenco puntato nel contesto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea una forma con testo che utilizzerà lo stile dell'elenco puntato
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Nota: L'applicazione reale dello stile dell'elenco puntato al testo richiederebbe chiamate API aggiuntive
                // non mostrato nella riflessione. Salveremo semplicemente la cartella di lavoro come dimostrazione.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



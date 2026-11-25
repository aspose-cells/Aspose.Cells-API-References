---
title: "TextOptions.Kerning"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "TextOptions property. Specifica la dimensione minima del carattere alla quale avverrà il kerning dei caratteri per questo blocco di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/kerning/
---
## TextOptions.Kerning property

Specifica la dimensione minima del carattere a cui avverrà il kerning dei caratteri per questo segmento di testo.

```csharp
public double Kerning { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyKerningDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo per dimostrare il kerning
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Kerning Demonstration Text";

            // Recupera le TextOptions della forma
            TextOptions textOptions = shape.TextOptions;

            // Mostra il valore corrente del kerning
            Console.WriteLine("Current Kerning value: " + textOptions.Kerning);

            // Imposta il kerning a 12 punti (dimensione minima del carattere affinché il kerning avvenga)
            textOptions.Kerning = 12;

            // Imposta una dimensione del carattere più grande per osservare l'effetto del kerning
            textOptions.Size = 24;

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("PropertyKerningDemo.xlsx");

            // Crea un'altra forma con un kerning diverso per il confronto
            var shape2 = worksheet.Shapes.AddTextBox(10, 0, 1, 0, 200, 100);
            shape2.Text = "Comparison Text Without Kerning";
            shape2.TextOptions.Size = 24;
            shape2.TextOptions.Kerning = 0; // No kerning

            // Salva nuovamente con entrambi gli esempi
            workbook.Save("PropertyKerningDemoWithComparison.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



---
title: "TextOptions.Spacing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextOptions. Specifica la spaziatura tra i caratteri all'interno di un blocco di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/spacing/
---
## TextOptions.Spacing property

Specifica la spaziatura tra i caratteri all'interno di un segmento di testo.

```csharp
public double Spacing { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertySpacingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 0, 100, 200);
            textBox.Text = "Sample Text with Spacing";

            // Ottieni le opzioni di testo della casella di testo
            TextOptions textOptions = textBox.TextOptions;

            // Visualizza il valore corrente della spaziatura
            Console.WriteLine("Current Spacing value: " + textOptions.Spacing);

            // Imposta nuovi valori di spaziatura e osserva gli effetti
            textOptions.Spacing = 2.0; // Increased spacing
            Console.WriteLine("Text with increased spacing (2.0)");

            // Salva la cartella di lavoro con la prima spaziatura
            workbook.Save("TextSpacingDemo1.xlsx");

            // Modifica la spaziatura a un valore negativo (caratteri più vicini tra loro)
            textOptions.Spacing = -1.0;
            Console.WriteLine("Text with decreased spacing (-1.0)");

            // Salva la cartella di lavoro con la seconda spaziatura
            workbook.Save("TextSpacingDemo2.xlsx");

            // Ripristina la spaziatura predefinita
            textOptions.Spacing = 0.0;
            Console.WriteLine("Text with default spacing (0.0)");

            // Salva la cartella di lavoro con la spaziatura predefinita
            workbook.Save("TextSpacingDemo3.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



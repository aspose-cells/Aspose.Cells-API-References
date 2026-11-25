---
title: "TextOptions.LatinName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "TextOptions property. Ottiene e imposta il nome latino"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/latinname/
---
## TextOptions.LatinName property

Ottiene e imposta il nome latino.

```csharp
public string LatinName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyLatinNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma per dimostrare le opzioni di testo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            shape.Text = "Sample Text";

            // Recupera le TextOptions dal primo paragrafo della forma
            TextOptions textOptions = shape.TextBody.TextParagraphs[0].TextOptions;

            // Mostra il valore corrente di LatinName
            Console.WriteLine("Current LatinName value: " + textOptions.LatinName);

            // Imposta un nuovo valore per LatinName
            textOptions.LatinName = "Times New Roman";

            // Crea un'altra forma per confrontare il rendering dei caratteri
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 3, 0, 100, 150);
            shape2.Text = "Comparison Text";
            shape2.TextBody.TextParagraphs[0].TextOptions.LatinName = "Arial";

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("PropertyLatinNameDemo.xlsx");

            // Mostra il nuovo valore di LatinName
            Console.WriteLine("New LatinName value: " + textOptions.LatinName);
        }
    }
}
```

### Vedi anche

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



---
title: "TextOptions.UnderlineColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextOptions. Ottiene o imposta il colore della sottolineatura"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

Ottiene o imposta il colore della sottolineatura.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo per dimostrare le opzioni di testo
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // Ottieni le TextOptions dalla forma
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // Visualizza il valore corrente di UnderlineColor
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // Imposta un nuovo UnderlineColor (poiché la proprietà è leggibile e scrivibile)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // Abilita la sottolineatura per vedere l'effetto
                textOptions.Underline = FontUnderlineType.Single;

                // Visualizza il nuovo valore di UnderlineColor
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // Salva la cartella di lavoro per vedere l'effetto
                workbook.Save("UnderlineColorDemo.xlsx");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



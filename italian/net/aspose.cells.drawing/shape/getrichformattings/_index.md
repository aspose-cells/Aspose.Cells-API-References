---
title: "Shape.GetRichFormattings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo."
type: docs
url: /it/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo.

```csharp
public FontSetting[] GetRichFormattings()
```

### Valore di ritorno

Tutti gli oggetti Characters

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo formattato (conteggio corretto dei parametri per AddRectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // Formatta parti del testo
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // Ottieni formattazioni di testo ricco
            FontSetting[] formattings = shape.GetRichFormattings();

            // Visualizza le informazioni di formattazione
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



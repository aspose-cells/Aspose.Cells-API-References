---
title: "FontSettingCollection.TextAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSettingCollection. Rappresenta l'impostazione di allineamento del corpo del testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/textalignment/
---
## FontSettingCollection.TextAlignment property

Rappresenta l'impostazione di allineamento del corpo del testo.

```csharp
public ShapeTextAlignment TextAlignment { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextAlignmentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            shape.Text = "Sample Text";

            // Accedi e modifica le proprietà TextAlignment
            var textAlignment = shape.TextBody.TextAlignment;
            
            Console.WriteLine("Default Margins (Points):");
            Console.WriteLine($"AutoMargin: {textAlignment.IsAutoMargin}");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");

            // Modifica i margini
            textAlignment.TopMarginPt = 36;
            textAlignment.BottomMarginPt = 36;
            textAlignment.LeftMarginPt = 18;
            textAlignment.RightMarginPt = 18;

            // Salva la cartella di lavoro
            workbook.Save("TextAlignmentDemo.xlsx");

            Console.WriteLine("\nModified Margins (Points):");
            Console.WriteLine($"Top: {textAlignment.TopMarginPt}");
            Console.WriteLine($"Bottom: {textAlignment.BottomMarginPt}");
            Console.WriteLine($"Left: {textAlignment.LeftMarginPt}");
            Console.WriteLine($"Right: {textAlignment.RightMarginPt}");
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../../shapetextalignment/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



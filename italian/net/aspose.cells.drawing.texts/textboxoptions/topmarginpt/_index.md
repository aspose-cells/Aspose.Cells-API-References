---
title: "TextBoxOptions.TopMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Ottiene e imposta il margine superiore in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

Ottiene e imposta il margine superiore in unità di Punti.

```csharp
public double TopMarginPt { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo al foglio di lavoro
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Imposta il margine superiore in punti
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // Salva la cartella di lavoro
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



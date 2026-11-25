---
title: "ShapeTextAlignment.NumberOfColumns"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Ottiene e imposta il numero di colonne di testo nel rettangolo di delimitazione"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Ottiene e imposta il numero di colonne di testo nel rettangolo di delimitazione.

```csharp
public int NumberOfColumns { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
            
            // Imposta il testo per la forma
            shape.Text = "This is sample text\nin multiple columns";
            
            // Accedi all'allineamento del testo e imposta il numero di colonne
            shape.TextBody.TextAlignment.NumberOfColumns = 2;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica la proprietà
            Console.WriteLine("Number of columns: " + 
                worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



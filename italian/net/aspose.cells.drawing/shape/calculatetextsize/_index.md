---
title: "Shape.CalculateTextSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ricalcola l'area del testo"
type: docs
url: /it/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Ricalcola l'area di testo

```csharp
public int[] CalculateTextSize()
```

### Valore di ritorno

Dimensione del testo in un array (larghezza e altezza).

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un testo di esempio alla cella A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Crea una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Imposta il testo nella forma
            shape.Text = "This is a test string to calculate text size";

            // Calcola la dimensione del testo
            int[] size = shape.CalculateTextSize();

            // Restituisci i risultati
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



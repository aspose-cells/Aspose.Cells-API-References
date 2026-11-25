---
title: "Shape.RemoveHyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Rimuove il collegamento ipertestuale della forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Rimuove il collegamento ipertestuale della forma.

```csharp
public void RemoveHyperlink()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta il collegamento ipertestuale
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Rimuovi il collegamento ipertestuale
            shape.RemoveHyperlink();

            // Verifica che il collegamento ipertestuale sia stato rimosso
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Salva la cartella di lavoro
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



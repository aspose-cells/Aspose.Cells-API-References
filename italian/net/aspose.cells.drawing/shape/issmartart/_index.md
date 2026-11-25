---
title: "Shape.IsSmartArt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se la forma è un smart art"
type: docs
url: /it/net/aspose.cells.drawing/shape/issmartart/
---
## Shape.IsSmartArt property

Indica se la forma è un SmartArt.

```csharp
public bool IsSmartArt { get; }
```

### Osservazioni

Solo per file ooxml.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsSmartArtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma SmartArt (Nota: Aspose.Cells non espone direttamente la creazione di SmartArt nelle versioni attuali)
            // Per dimostrazione, verificheremo le forme esistenti
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Verifica se la forma è SmartArt
            if (shape.IsSmartArt)
            {
                Console.WriteLine("The shape is a SmartArt object");
            }
            else
            {
                Console.WriteLine("The shape is not a SmartArt object");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



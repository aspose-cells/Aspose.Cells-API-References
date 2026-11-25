---
title: "Shape.GetResultOfSmartArt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Conversione di smart art in forme raggruppate"
type: docs
url: /it/net/aspose.cells.drawing/shape/getresultofsmartart/
---
## Shape.GetResultOfSmartArt method

Conversione della grafica intelligente in forme raggruppate.

```csharp
public virtual GroupShape GetResultOfSmartArt()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetResultOfSmartArtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare (poiché non possiamo creare SmartArt direttamente)
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 200, 200, 0, 0);
            
            // In uno scenario reale, caricheremmo una forma SmartArt esistente
            // Per scopi dimostrativi, salteremo il controllo IsSmartArt poiché non possiamo impostarlo

            // Ottieni il risultato di SmartArt (funzionerebbe solo se la forma fosse effettivamente SmartArt)
            GroupShape groupShape = shape.GetResultOfSmartArt();
            Console.WriteLine("Converted shape to GroupShape");
        }
    }
}
```

### Vedi anche

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



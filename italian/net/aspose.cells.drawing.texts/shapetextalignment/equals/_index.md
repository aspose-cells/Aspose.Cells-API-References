---
title: "ShapeTextAlignment.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeTextAlignment. Determina se questa istanza ha lo stesso valore di un altro oggetto ShapeTextAlignment specificato"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Determina se questa istanza ha lo stesso valore di un altro oggetto [`ShapeTextAlignment`](../) specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | L'oggetto [`ShapeTextAlignment`](../) da confrontare con questa istanza. |

### Valore di ritorno

true se il valore del parametro obj è lo stesso del valore di questa istanza; altrimenti, false. Se obj è null, questo metodo restituisce false.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma per confrontare l'allineamento del testo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Ottieni l'allineamento del testo di un'altra forma per il confronto
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)



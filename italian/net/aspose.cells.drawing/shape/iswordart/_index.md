---
title: "Shape.IsWordArt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se questa forma è un WordArt"
type: docs
url: /it/net/aspose.cells.drawing/shape/iswordart/
---
## Shape.IsWordArt property

Indica se questa forma è un WordArt.

```csharp
public bool IsWordArt { get; }
```

### Osservazioni

Solo per la forma Legacy di file xls.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsWordArtDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma WordArt con tutti i parametri richiesti
            Shape wordArt = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample WordArt", 0, 0, 100, 100, 100, 100);

            // Aggiungi una forma rettangolare regolare con tutti i parametri richiesti
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 150, 100, 100, 100);

            // Verifica se le forme sono WordArt
            Console.WriteLine("WordArt shape is WordArt: " + wordArt.IsWordArt);
            Console.WriteLine("Rectangle shape is WordArt: " + rectangle.IsWordArt);

            // Esempio di utilizzo della proprietà IsWordArt
            if (wordArt.IsWordArt)
            {
                Console.WriteLine("First shape is a WordArt object");
            }

            if (!rectangle.IsWordArt)
            {
                Console.WriteLine("Second shape is not a WordArt object");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



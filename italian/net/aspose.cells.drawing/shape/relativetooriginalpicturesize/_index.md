---
title: "Shape.RelativeToOriginalPictureSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se la forma è relativa alle dimensioni dell'immagine originale"
type: docs
url: /it/net/aspose.cells.drawing/shape/relativetooriginalpicturesize/
---
## Shape.RelativeToOriginalPictureSize property

Indica se la forma è relativa alle dimensioni originali dell'immagine.

```csharp
public bool RelativeToOriginalPictureSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRelativeToOriginalPictureSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'immagine al foglio di lavoro
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Accedi alle proprietà della forma - Picture è già una Shape, non è necessario eseguire il cast
            Shape shape = picture;

            // Dimostra la proprietà RelativeToOriginalPictureSize
            Console.WriteLine("Original RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
            
            // Modifica la proprietà
            shape.RelativeToOriginalPictureSize = !shape.RelativeToOriginalPictureSize;
            Console.WriteLine("Modified RelativeToOriginalPictureSize: " + shape.RelativeToOriginalPictureSize);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



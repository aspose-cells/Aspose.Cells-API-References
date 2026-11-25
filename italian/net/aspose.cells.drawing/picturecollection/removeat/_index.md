---
title: "PictureCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PictureCollection. Rimuove le forme all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Rimuove le forme all'indice specifico

```csharp
public void RemoveAt(int index)
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune immagini al foglio di lavoro
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Rimuovi l'immagine all'indice specificato
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Vedi anche

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



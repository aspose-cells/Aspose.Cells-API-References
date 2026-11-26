---
title: "PictureCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PictureCollection. Elimina formas en el índice específico"
type: docs
url: /es/net/aspose.cells.drawing/picturecollection/removeat/
---
## PictureCollection.RemoveAt method

Eliminar shapes en el índice específico

```csharp
public void RemoveAt(int index)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PictureCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir algunas imágenes a la hoja de cálculo
            int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
            int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
            int index3 = worksheet.Pictures.Add(10, 1, "image3.png");

            Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);

            // Eliminar la imagen en el índice especificado
            worksheet.Pictures.RemoveAt(index2);

            Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



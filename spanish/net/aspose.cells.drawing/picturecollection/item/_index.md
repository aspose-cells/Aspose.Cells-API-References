---
title: "PictureCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PictureCollection. Obtiene el elemento Picture en el índice especificado"
type: docs
url: /es/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Obtiene el elemento [`Picture`](../../picture/) en el índice especificado.

```csharp
public Picture this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la colección de imágenes
            PictureCollection pictures = worksheet.Pictures;
            
            // Añadir una imagen (reemplaza "image.png" con la ruta real de la imagen)
            int index = pictures.Add(1, 1, "image.png");
            
            // Acceder a la imagen usando la propiedad Item
            Picture pic = pictures[index];
            
            // Demostrar el uso de la propiedad Item
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Modificar propiedades de la imagen
            pic.Height = 200;
            pic.Width = 300;
            
            // Guarda el libro de trabajo
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



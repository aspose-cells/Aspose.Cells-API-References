---
title: "Picture.IsAutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. True indica que el tamaño del objeto ole se cambiará automáticamente al tamaño de la instantánea del contenido incrustado cuando se active el objeto ole"
type: docs
url: /es/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

True indica que el tamaño del objeto ole se cambiará automáticamente al tamaño de la instantánea del contenido incrustado cuando se active el objeto ole.

```csharp
public bool IsAutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Demostrar la propiedad IsAutoSize
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Establecer IsAutoSize a true - la imagen se redimensionará automáticamente para ajustarse a su contenido
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Establecer IsAutoSize a false - la imagen mantendrá sus dimensiones originales
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Guarda el libro de trabajo
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



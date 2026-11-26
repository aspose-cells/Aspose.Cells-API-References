---
title: "Picture.IsDynamicDataExchange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene o establece si hay intercambio dinámico de datos"
type: docs
url: /es/net/aspose.cells.drawing/picture/isdynamicdataexchange/
---
## Picture.IsDynamicDataExchange property

Obtiene o establece si hay intercambio dinámico de datos

```csharp
public bool IsDynamicDataExchange { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsDynamicDataExchangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Demuestra la propiedad IsDynamicDataExchange
            Console.WriteLine("Original IsDynamicDataExchange value: " + picture.IsDynamicDataExchange);
            
            // Establece IsDynamicDataExchange a true
            picture.IsDynamicDataExchange = true;
            Console.WriteLine("After setting IsDynamicDataExchange to true: " + picture.IsDynamicDataExchange);

            // Guarda el libro de trabajo
            workbook.Save("PicturePropertyIsDynamicDataExchangeDemo.xlsx", SaveFormat.Xlsx);

            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("PicturePropertyIsDynamicDataExchangeDemo.xlsx");
            Picture loadedPicture = loadedWorkbook.Worksheets[0].Pictures[0];
            Console.WriteLine("Loaded IsDynamicDataExchange value: " + loadedPicture.IsDynamicDataExchange);
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



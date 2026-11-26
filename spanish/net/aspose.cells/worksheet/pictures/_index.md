---
title: "Worksheet.Pictures"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene una colección de Picture"
type: docs
url: /es/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

Obtiene una colección de [`Picture`](../../../aspose.cells.drawing/picture/).

```csharp
public PictureCollection Pictures { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Establecer propiedades de la imagen
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Cargar el libro de trabajo guardado para verificar
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### Ver también

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Picture.PlaceInCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Picture. Coloca esta imagen en la celda"
type: docs
url: /es/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Coloca esta imagen en la celda

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Picture.IsPlacedInCell. Esta propiedad será eliminada 12 meses después desde enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Coloca la imagen en la celda A1
            picture.PlaceInCell();

            // Verifica que la imagen esté colocada en la celda
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



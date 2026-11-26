---
title: "MsoFormatPicture.TransparentColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Obtiene y establece el color transparente de la imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/transparentcolor/
---
## MsoFormatPicture.TransparentColor property

Obtiene y establece el color transparente de la imagen.

```csharp
public CellsColor TransparentColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparentColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen de ejemplo (usando un rectángulo de color sólido como ejemplo)
            int pictureIndex = worksheet.Pictures.Add(0, 0, "sample.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Establecer color transparente
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.Blue;
            picture.FormatPicture.TransparentColor = transparentColor;

            // Obtener y mostrar el color transparente
            CellsColor currentTransparentColor = picture.FormatPicture.TransparentColor;
            Console.WriteLine("Current transparent color: " + currentTransparentColor.Color);

            // Guarda el libro de trabajo
            workbook.Save("TransparentColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "Clase MsoFormatPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.MsoFormatPicture class. Representa el formato de imagen"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Representa el formato de imagen.

```csharp
public class MsoFormatPicture
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Representa la ubicación del borde inferior del rectángulo de recorte, expresada como una proporción de la altura de la imagen. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Representa la ubicación del borde inferior del rectángulo de recorte, en unidades de pulgadas. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Representa la modificación de brillo de la imagen en unidades de porcentaje. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Representa la modificación de contraste de la imagen en unidades de porcentaje. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Representa la gamma de la imagen. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Indica si esta imagen debe mostrarse en blanco y negro de dos colores. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Indica si esta imagen debe mostrarse en escala de grises. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Representa la ubicación del borde izquierdo del rectángulo de recorte, expresada como una proporción del ancho de la imagen. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Representa la ubicación del borde izquierdo del rectángulo de recorte, en unidades de pulgadas. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Representa la ubicación del borde derecho del rectángulo de recorte, expresada como una proporción del ancho de la imagen. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Representa la ubicación del borde derecho del rectángulo de recorte, en unidades de pulgadas. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Representa la ubicación del borde superior del rectángulo de recorte, expresada como una proporción de la altura de la imagen. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Representa la ubicación del borde superior del rectángulo de recorte, en unidades de pulgadas. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Obtiene y establece el color transparente de la imagen. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Obtiene el código hash. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPictureDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Accede al objeto MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Establece propiedades de MsoFormatPicture
            formatPicture.TopCropInch = 0.5;
            formatPicture.BottomCropInch = 0.5;
            formatPicture.LeftCropInch = 0.5;
            formatPicture.RightCropInch = 0.5;
            formatPicture.Transparency = 0.5;
            formatPicture.Contrast = 0.8;
            formatPicture.Brightness = 0.6;
            formatPicture.Gamma = 1.0;
            formatPicture.IsBiLevel = false;
            formatPicture.IsGray = false;

            // Establece el color transparente
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Guarda el libro de trabajo
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



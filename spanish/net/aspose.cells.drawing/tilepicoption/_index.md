---
title: "Clase TilePicOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.TilePicOption. Representa una imagen de mosaico como textura"
type: docs
url: /es/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Representa una imagen en mosaico como textura.

```csharp
public class TilePicOption
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TilePicOption](tilepicoption/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Obtiene o establece la alineación para el mosaico. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Obtiene o establece el tipo de espejo para el mosaico. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Obtiene o establece el desplazamiento X para la imagen de mosaico. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Obtiene o establece el desplazamiento Y para la imagen de mosaico. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Obtiene o establece la escala X para la imagen de mosaico. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Obtiene o establece la escala Y para la imagen de mosaico. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un gráfico para demostración
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer el tipo de relleno a textura
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Cargar imagen de ejemplo (reemplazar con la ruta real)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Crear y configurar TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Guarda el libro de trabajo
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



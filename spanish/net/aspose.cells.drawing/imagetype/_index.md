---
title: "Enum ImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ImageType enum. Especifica el formato de tipo de una imagen"
type: docs
url: /es/net/aspose.cells.drawing/imagetype/
---
## ImageType enumeration

Especifica el tipo (formato) de una imagen.

```csharp
public enum ImageType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Unknown | `0` | Un tipo de imagen desconocido. |
| Emf | `2` | Metarchivo mejorado de Windows. |
| Wmf | `3` | Metarchivo de Windows. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Portable Network Graphics. |
| Bmp | `7` | Mapa de bits de Windows |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile que es más compatible con Office. |
| WebP | `72` | Formato de imagen Weppy |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ImageTypeDemo
    {
        public static void ImageTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Guarde el gráfico como una imagen en diferentes formatos
            chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
            chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
            chart.ToImage("ChartImagePng.png", ImageType.Png);
            chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
            chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
            chart.ToImage("ChartImageGif.gif", ImageType.Gif);
            chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
            chart.ToImage("ChartImageSvg.svg", ImageType.Svg);

            // Genere la salida de los resultados
            Console.WriteLine("Chart images saved in various formats.");

            // Guarda el libro de trabajo
            workbook.Save("ImageTypeExample.xlsx");
            workbook.Save("ImageTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



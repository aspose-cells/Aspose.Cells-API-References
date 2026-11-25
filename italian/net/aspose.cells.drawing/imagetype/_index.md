---
title: "Enum ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ImageType. Specifica il formato di tipo di un'immagine"
type: docs
url: /it/net/aspose.cells.drawing/imagetype/
---
## ImageType enumeration

Specifica il tipo (formato) di un'immagine.

```csharp
public enum ImageType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Unknown | `0` | Un tipo di immagine sconosciuto. |
| Emf | `2` | Metafile migliorato di Windows. |
| Wmf | `3` | Metafile Windows. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Grafica di rete portatile. |
| Bmp | `7` | Bitmap di Windows |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile che è più compatibile con Office. |
| WebP | `72` | Formato immagine Weppy |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Salva il grafico come immagine in diversi formati
            chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
            chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
            chart.ToImage("ChartImagePng.png", ImageType.Png);
            chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
            chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
            chart.ToImage("ChartImageGif.gif", ImageType.Gif);
            chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
            chart.ToImage("ChartImageSvg.svg", ImageType.Svg);

            // Restituisci i risultati
            Console.WriteLine("Chart images saved in various formats.");

            // Salva la cartella di lavoro
            workbook.Save("ImageTypeExample.xlsx");
            workbook.Save("ImageTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



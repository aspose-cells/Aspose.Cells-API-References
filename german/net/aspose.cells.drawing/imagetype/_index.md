---
title: "Enum ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ImageType enum. Gibt das Format eines Bildes an."
type: docs
url: /de/net/aspose.cells.drawing/imagetype/
---
## ImageType enumeration

Gibt den Typ (Format) eines Bildes an.

```csharp
public enum ImageType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Unknown | `0` | Ein unbekannter Bildtyp. |
| Emf | `2` | Windows Enhanced Metafile. |
| Wmf | `3` | Windows-Metadatei. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Portable Network Graphics. |
| Bmp | `7` | Windows Bitmap |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile, das mit Office besser kompatibel ist. |
| WebP | `72` | Weppy-Bildformat |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Speichern Sie das Diagramm als Bild in verschiedenen Formaten
            chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
            chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
            chart.ToImage("ChartImagePng.png", ImageType.Png);
            chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
            chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
            chart.ToImage("ChartImageGif.gif", ImageType.Gif);
            chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
            chart.ToImage("ChartImageSvg.svg", ImageType.Svg);

            // Ergebnisse ausgeben
            Console.WriteLine("Chart images saved in various formats.");

            // Speichere die Arbeitsmappe
            workbook.Save("ImageTypeExample.xlsx");
            workbook.Save("ImageTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



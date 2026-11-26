---
title: "Перечисление ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.ImageType. Указывает формат типа изображения"
type: docs
url: /ru/net/aspose.cells.drawing/imagetype/
---
## ImageType enumeration

Указывает тип (формат) изображения.

```csharp
public enum ImageType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Unknown | `0` | Неизвестный тип изображения. |
| Emf | `2` | Windows Enhanced Metafile. |
| Wmf | `3` | Windows Metafile. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Portable Network Graphics. |
| Bmp | `7` | Windows Bitmap |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile, более совместимый с Office. |
| WebP | `72` | Формат изображения Weppy |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            // Сохранить диаграмму как изображение в разных форматах
            chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
            chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
            chart.ToImage("ChartImagePng.png", ImageType.Png);
            chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
            chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
            chart.ToImage("ChartImageGif.gif", ImageType.Gif);
            chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
            chart.ToImage("ChartImageSvg.svg", ImageType.Svg);

            // Выведите результаты
            Console.WriteLine("Chart images saved in various formats.");

            // Сохраните книгу
            workbook.Save("ImageTypeExample.xlsx");
            workbook.Save("ImageTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



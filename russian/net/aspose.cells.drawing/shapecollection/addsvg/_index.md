---
title: "ShapeCollection.AddSvg"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет svg‑изображение"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Добавляет SVG‑изображение.

```csharp
public Picture AddSvg(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] svgData, byte[] compatibleImageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение фигуры от её левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Горизонтальное смещение фигуры от её левого столбца, в пикселях. |
| высота | Int32 | Высота фигуры, в пикселях. |
| ширина | Int32 | Ширина фигуры, в пикселях. |
| svgData | Byte[] | Данные svg‑изображения. |
| compatibleImageData | Byte[] | Преобразованные данные изображения из svg, совместимые с Excel 2016 или более ранними версиями. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSvgWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Drawing.ShapeCollection shapes = worksheet.Shapes;

            // Load SVG file
            using (FileStream fs = new FileStream("image.svg", FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                
                // Add SVG to worksheet
                Aspose.Cells.Drawing.Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



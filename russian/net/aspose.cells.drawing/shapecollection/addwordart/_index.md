---
title: "ShapeCollection.AddWordArt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет предустановленный WordArt, начиная с Excel 2007."
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Добавляет предустановленный WordArt, начиная с Excel 2007.s

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | PresetWordArtStyle | Предустановленный стиль WordArt. |
| текст | String | Текст. |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение фигуры от её левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение фигуры от её левой колонки, в пикселях. |
| высота | Int32 | Представляет высоту фигуры в пикселях. |
| ширина | Int32 | Представляет ширину фигуры, в пикселях. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;

            // Добавить WordArt с указанными параметрами
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Сохраните книгу
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



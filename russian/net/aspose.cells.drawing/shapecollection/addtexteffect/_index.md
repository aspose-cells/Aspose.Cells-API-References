---
title: "ShapeCollection.AddTextEffect"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Вставляет объект WordArt"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Вставляет объект WordArt.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| эффект | MsoPresetTextEffect | Тип предустановленного текстового эффекта mso. |
| текст | String | Текст WordArt. |
| fontName | String | Имя шрифта. |
| размер | Int32 | Размер шрифта |
| fontBold | Boolean | Указывает, является ли шрифт полужирным. |
| fontItalic | Boolean | Указывает, является ли шрифт курсивом. |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение фигуры от её левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Представляет горизонтальное смещение фигуры от её левой колонки, в пикселях. |
| высота | Int32 | Представляет высоту фигуры в пикселях. |
| ширина | Int32 | Представляет ширину фигуры, в пикселях. |

### Возвращаемое значение

Возвращает объект Shape, представляющий новый объект WordArt.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



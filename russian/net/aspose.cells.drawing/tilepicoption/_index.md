---
title: "Класс TilePicOption"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.TilePicOption. Представляет изображение плитки в виде текстуры"
type: docs
url: /ru/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Представляет изображение плитки в виде текстуры.

```csharp
public class TilePicOption
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Получает или задает выравнивание для замощения. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Получает или задает тип зеркального отражения для замощения. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Получает или задает смещение по оси X для изображения замощения. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Получает или задает смещение по оси Y для изображения замощения. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Получает или задает масштаб по оси X для изображения замощения. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Получает или задает масштаб по оси Y для изображения замощения. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить диаграмму для демонстрации
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Установить тип заливки как текстуру
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Загрузить пример изображения (заменить реальным путем)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Создать и настроить TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Сохраните книгу
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



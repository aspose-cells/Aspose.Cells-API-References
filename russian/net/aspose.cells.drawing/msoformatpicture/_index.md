---
title: "Класс MsoFormatPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.MsoFormatPicture класс. Представляет формат изображения"
type: docs
url: /ru/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Представляет формат изображения.

```csharp
public class MsoFormatPicture
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Представляет расположение нижней части прямоугольника обрезки, выраженное как отношение к высоте изображения. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Представляет расположение нижней части прямоугольника обрезки, в дюймах. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Представляет изменение яркости изображения в процентах. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Представляет изменение контрастности изображения в процентах. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Представляет гамму изображения. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Указывает, должно ли это изображение отображаться в двухцветном черно-белом режиме. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Указывает, должно ли это изображение отображаться в градациях серого. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Представляет расположение левой стороны прямоугольника обрезки, выраженное как отношение к ширине изображения. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Представляет расположение левой стороны прямоугольника обрезки, в дюймах. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Представляет расположение правой стороны прямоугольника обрезки, выраженное как отношение к ширине изображения. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Представляет расположение правой стороны прямоугольника обрезки, в дюймах. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Представляет расположение верхней части прямоугольника обрезки, выраженное как отношение к высоте изображения. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Представляет расположение верхней части прямоугольника обрезки, в дюймах. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Получает и задает прозрачный цвет изображения. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Получает хеш‑код. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Получить доступ к объекту MsoFormatPicture
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Установить свойства MsoFormatPicture
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

            // Установить прозрачный цвет
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Сохраните книгу
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



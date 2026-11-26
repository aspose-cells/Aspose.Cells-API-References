---
title: "Класс FillFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.FillFormat. Инкапсулирует объект, представляющий формат заливки для фигуры."
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Инкапсулирует объект, представляющий формат заливки формы.

```csharp
public class FillFormat
```

## Свойства

| Имя | Описание |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype/) { get; set; } | Получает и задает тип заливки. |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1/) { get; } | Возвращает градиентный цвет 1 для указанной заливки. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2/) { get; } | Возвращает градиентный цвет 2 для указанной заливки. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype/) { get; } | Возвращает тип градиентного цвета для указанной заливки. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree/) { get; } | Возвращает степень градиента для указанного заполнения. Применяется только для Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill/) { get; } | Получает объект [`GradientFill`](./gradientfill/). |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle/) { get; } | Возвращает стиль градиента для указанного заполнения. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant/) { get; } | Возвращает вариант градиента для указанного заполнения. Применяется только для Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata/) { get; set; } | Получает и задает данные изображения картинки. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern/) { get; set; } | Представляет шаблон отображения области. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill/) { get; } | Получает объект [`PatternFill`](./patternfill/). |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype/) { get; set; } | Получает и задает тип формата изображения. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor/) { get; } | Возвращает предустановленный цвет градиента для указанного заполнения. |
| [Scale](../../aspose.cells.drawing/fillformat/scale/) { get; set; } | Получает и задает масштаб формата изображения. |
| [SetType](../../aspose.cells.drawing/fillformat/settype/) { get; set; } | (**Obsolete.**) Получает тип набора формата заполнения. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill/) { get; } | Получает объект [`SolidFill`](./solidfill/). |
| [Texture](../../aspose.cells.drawing/fillformat/texture/) { get; set; } | Представляет тип текстуры для указанного заполнения. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill/) { get; } | Получает объект [`TextureFill`](./texturefill/). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency/) { get; set; } | Возвращает или задает степень прозрачности области значением от 0.0 (непрозрачный) до 1.0 (прозрачный). |
| [Type](../../aspose.cells.drawing/fillformat/type/) { get; set; } | (**Obsolete.**) Получает и задает тип заполнения. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode/)() | Получает хеш‑код. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Устанавливает указанное заполнение в одноцветный градиент. Применяется только для Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient/)(GradientPresetType, GradientStyleType, int) | Устанавливает указанное заполнение в градиент с предустановленным цветом. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Устанавливает указанное заполнение в двухцветный градиент. Применяется только для Excel 2007. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");
            
            // Добавить столбчатую диаграмму на лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте серию данных в диаграмму
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";
            
            // Применить градиентную заливку к области серии
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(System.Drawing.Color.Lime, 1, 
                GradientStyleType.Horizontal, 1);
            
            // Сохраните книгу
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



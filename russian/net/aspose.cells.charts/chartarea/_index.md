---
title: "Класс ChartArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.ChartArea. Инкапсулирует объект, представляющий область диаграммы в листе."
type: docs
url: /ru/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Инкапсулирует объект, представляющий область диаграммы в листе.

```csharp
public class ChartArea : ChartFrame
```

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Получает [`area`](../chartframe/area/). (Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Получает и задает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) Получает и задает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях. (Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Получает [`border`](../../aspose.cells.drawing/line/). (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Представляет высоту положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Представляет высоту положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Представляет ширину положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Представляет ширину положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Представляет координату x положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Представляет координату x положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Представляет координату y положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Представляет координату y положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| override [Font](../../aspose.cells.charts/chartarea/font/) { get; } | Получает объект [`Font`](./font/) указанного объекта ChartArea. |
| override [Height](../../aspose.cells.charts/chartarea/height/) { get; set; } | (**Obsolete.**) Получает или задает вертикальное смещение от строки нижнего‑правого угла, в единицах 1/4000 области диаграммы. |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Получает или задает высоту кадра в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [HeightRatioToChart](../../aspose.cells.charts/chartarea/heightratiotochart/) { get; set; } | Получает или задает вертикальное смещение от строки нижнего правого угла, в виде отношения к области диаграммы. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Указывает, автоматически ли задаются размеры кадра диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Указывает, включает ли размер области построения отметки делений и подписи осей. Значение False указывает, что размер определяет только область построения, без отметок делений и подписей осей.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True, если у кадра есть тень.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Получает объект [`ShapeProperties`](../chartframe/shapeproperties/).(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Получает объект [`Font`](../chartframe/font/) указанного объекта ChartFrame.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Получает и задает параметры текста.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [Width](../../aspose.cells.charts/chartarea/width/) { get; set; } | (**Obsolete.**) Получает или задает горизонтальное смещение от столбца нижнего правого угла, в единицах 1/4000 области диаграммы. |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Получает или задает ширину рамки в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [WidthRatioToChart](../../aspose.cells.charts/chartarea/widthratiotochart/) { get; set; } | Получает или задает горизонтальное смещение от столбца нижнего правого угла, в виде отношения к области диаграммы. |
| override [X](../../aspose.cells.charts/chartarea/x/) { get; set; } | (**Obsolete.**) Получает или задает горизонтальное смещение от столбца верхнего‑левого угла, в единицах 1/4000 области диаграммы. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Получает или задает координату x верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [XRatioToChart](../../aspose.cells.charts/chartarea/xratiotochart/) { get; set; } | Получает или задает горизонтальное смещение от столбца верхнего‑левого угла, как отношение к области диаграммы. |
| override [Y](../../aspose.cells.charts/chartarea/y/) { get; set; } | (**Obsolete.**) Получает или получает вертикальное смещение от строки верхнего левого угла, в единицах 1/4000 области диаграммы. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Получает или задает координату y верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [YRatioToChart](../../aspose.cells.charts/chartarea/yratiotochart/) { get; set; } | Получает или получает вертикальное смещение от строки верхнего левого угла, в виде отношения к области диаграммы. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Устанавливает позицию рамки в автоматический режим(Наследовано от [`ChartFrame`](../chartframe/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartAreaDemo
    {
        public static void ChartAreaExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление примерного значения в ячейку "A1"
            worksheet.Cells["A1"].PutValue(50);

            // Добавление примерного значения в ячейку "A2"
            worksheet.Cells["A2"].PutValue(100);

            // Добавление примерного значения в ячейку "A3"
            worksheet.Cells["A3"].PutValue(150);

            // Добавление примерного значения в ячейку "B1"
            worksheet.Cells["B1"].PutValue(60);

            // Добавление примерного значения в ячейку "B2"
            worksheet.Cells["B2"].PutValue(32);

            // Добавление примерного значения в ячейку "B3"
            worksheet.Cells["B3"].PutValue(50);

            // Добавление диаграммы в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // Получение экземпляра недавно добавленной диаграммы
            Chart chart = worksheet.Charts[chartIndex];

            // Добавление NSeries (источника данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
            chart.NSeries.Add("A1:B3", true);

            // Получение области диаграммы
            ChartArea chartArea = chart.ChartArea;

            // Установка свойств ChartArea
            chartArea.X = 10;
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;
            chartArea.IsInnerMode = false;
            chartArea.AutoScaleFont = true;
            chartArea.BackgroundMode = BackgroundMode.Transparent;
            chartArea.IsAutomaticSize = true;
            chartArea.Shadow = true;

            // Установка цвета переднего плана области диаграммы
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Сохранение файла Excel
            workbook.Save("ChartAreaExample.xlsx");
            workbook.Save("ChartAreaExample.pdf");
        }
    }
}
```

### См. также

* class [ChartFrame](../chartframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



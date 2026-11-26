---
title: "Класс Legend"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Legend. Инкапсулирует объект, представляющий легенду диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/legend/
---
## Legend class

Инкапсулирует объект, представляющий легенду диаграммы.

```csharp
public class Legend : ChartTextFrame
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
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | Получает и задает направление текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | Получает объект [`Font`](../chartframe/font/) указанного объекта ChartFrame.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Получает или задает высоту кадра в единицах 1/4000 области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Получает или задает высоту кадра в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Получает или задает высоту кадра в единицах отношения к области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Указывает, автоматически ли вращается текст диаграммы.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Указывает, автоматически ли задаются размеры кадра диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | Указывает, что текст генерируется автоматически.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Указывает, удалена ли эта метка данных.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Указывает, включает ли размер области построения отметки делений и подписи осей. Значение False указывает, что размер определяет только область построения, без отметок делений и подписей осей.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay/) { get; set; } | Получает или задает, отображать ли легенду без перекрытия диаграммы. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Получает или задает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это масштабирование текста внутри формы для размещения всего текста внутри.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Получает или задает значение, указывающее, переносится ли текст.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries/) { get; } | Получает коллекцию всех объектов LegendEntry в указанной легенде диаграммы. Установка записей легенды для поверхностной диаграммы не поддерживается. Поэтому будет возвращено null, если тип диаграммы — поверхностный. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels/) { get; } | (**Obsolete.**) Получает подписи записей легенды после вызова метода Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Получает и задает ссылку на лист рабочей книги.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [Position](../../aspose.cells.charts/legend/position/) { get; set; } | Получает или задает тип положения легенды. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Представляет порядок чтения текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Представляет угол поворота текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True, если у кадра есть тень.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Получает объект [`ShapeProperties`](../chartframe/shapeproperties/).(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [Text](../../aspose.cells.charts/charttextframe/text/) { get; set; } | Получает или задает текст заголовка кадра. (Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Представляет порядок чтения текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Получает объект [`Font`](../chartframe/font/) указанного объекта ChartFrame.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Получает и задает горизонтальное выравнивание текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Получает и задает параметры текста.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Получает или задает вертикальное выравнивание текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Получает или задает ширину рамки в единицах 1/4000 области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Получает или задает ширину рамки в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Получает или задает ширину рамки в единицах отношения области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Получает или задает координату x верхнего левого угла в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Получает или задает координату x верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Получает или задает координату x верхнего левого угла в единицах отношения к области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Получает или задает координату y верхнего левого угла в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Получает или задает координату y верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Получает или задает координату y верхнего левого угла в единицах отношения к области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Возвращает объект Characters, представляющий диапазон символов внутри текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [GetLegendLabels](../../aspose.cells.charts/legend/getlegendlabels/)() | Получает подписи записей легенды после вызова метода Chart.Calculate(). |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Устанавливает позицию рамки в автоматический режим(Наследовано от [`ChartFrame`](../chartframe/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class LegendDemo
    {
        public static void LegendExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить первый лист
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Добавить диаграмму в лист
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Получите доступ к легенде диаграммы
            Legend legend = chart.Legend;

            // Установить свойства легенды
            legend.Position = LegendPositionType.Left;
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;
            legend.IsOverLay = false;
            legend.IsAutoText = true;
            legend.IsDeleted = false;
            legend.TextHorizontalAlignment = TextAlignmentType.Center;
            legend.TextVerticalAlignment = TextAlignmentType.Center;
            legend.RotationAngle = 0;
            legend.Text = "Legend Text";
            legend.LinkedSource = "Sheet1!A1";
            legend.TextDirection = TextDirectionType.LeftToRight;
            legend.ReadingOrder = TextDirectionType.Context;
            legend.DirectionType = ChartTextDirectionType.Horizontal;
            legend.IsTextWrapped = true;
            legend.IsResizeShapeToFitText = true;
            legend.IsInnerMode = false;
            legend.AutoScaleFont = true;
            legend.BackgroundMode = BackgroundMode.Transparent;
            legend.IsAutomaticSize = true;
            legend.X = 100;
            legend.Y = 100;
            legend.Height = 200;
            legend.Width = 200;
            legend.Shadow = true;

            // Сохраните книгу
            workbook.Save("LegendExample.xlsx");
            workbook.Save("LegendExample.pdf");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



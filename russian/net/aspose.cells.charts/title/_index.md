---
title: "Класс Title"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.Title. Инкапсулирует объект, представляющий заголовок диаграммы или оси"
type: docs
url: /ru/net/aspose.cells.charts/title/
---
## Title class

Инкапсулирует объект, представляющий заголовок диаграммы или оси.

```csharp
public class Title : ChartTextFrame
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
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Получает или задает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это масштабирование текста внутри формы для размещения всего текста внутри.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Получает или задает значение, указывающее, переносится ли текст.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [IsVisible](../../aspose.cells.charts/title/isvisible/) { get; set; } | Представляет, видим ли заголовок. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Получает и задает ссылку на лист рабочей книги.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [OverLay](../../aspose.cells.charts/title/overlay/) { get; set; } | Представляет наложенный центрированный заголовок на диаграмме без изменения её размеров. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Представляет порядок чтения текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Представляет угол поворота текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True, если у кадра есть тень.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Получает объект [`ShapeProperties`](../chartframe/shapeproperties/).(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/title/text/) { get; set; } | Получает или задает текст метки единицы отображения. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Представляет порядок чтения текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Получает объект [`Font`](../chartframe/font/) указанного объекта ChartFrame.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Получает и задает горизонтальное выравнивание текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Получает и задает параметры текста.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Получает или задает вертикальное выравнивание текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Получает или задает ширину рамки в единицах 1/4000 области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Получает или задает ширину рамки в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Получает или задает ширину рамки в единицах отношения области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [X](../../aspose.cells.charts/title/x/) { get; set; } | (**Obsolete.**) Получает или задает координату X верхнего левого угла в единицах 1/4000 области диаграммы. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Получает или задает координату x верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [XRatioToChart](../../aspose.cells.charts/title/xratiotochart/) { get; set; } | Получает или задает координату x верхнего левого угла в единицах доли области диаграммы. X в пикселях = XRatioToChart * Chart.ChartObject.Width; |
| override [Y](../../aspose.cells.charts/title/y/) { get; set; } | (**Obsolete.**) Получает или задает координату y верхнего левого угла в единицах 1/4000 области диаграммы. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Получает или задает координату y верхнего левого угла в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [YRatioToChart](../../aspose.cells.charts/title/yratiotochart/) { get; set; } | Получает или задает координату y верхнего левого угла в единицах доли области диаграммы. Y в пикселях = YRatioToChart * Chart.ChartObject.Width; |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters/#characters_1)() | Получает форматирование текста этого заголовка. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Возвращает объект Characters, представляющий диапазон символов внутри текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Устанавливает позицию рамки в автоматический режим(Наследовано от [`ChartFrame`](../chartframe/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TitleDemo
    {
        public static void TitleExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
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

            // Установить источник данных для диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить заголовок диаграммы
            chart.Title.Text = "Income Analysis";
            chart.Title.Font.Color = Color.Blue;
            chart.Title.IsVisible = true;
            chart.Title.X = 100;
            chart.Title.Y = 50;
            chart.Title.OverLay = false;
            chart.Title.IsAutoText = false;
            chart.Title.IsDeleted = false;
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Center;
            chart.Title.RotationAngle = 0;
            chart.Title.LinkedSource = null;
            chart.Title.TextDirection = TextDirectionType.LeftToRight;
            chart.Title.ReadingOrder = TextDirectionType.LeftToRight;
            chart.Title.DirectionType = ChartTextDirectionType.Horizontal;
            chart.Title.IsTextWrapped = true;
            chart.Title.IsResizeShapeToFitText = true;
            chart.Title.IsInnerMode = false;
            chart.Title.AutoScaleFont = true;
            chart.Title.BackgroundMode = BackgroundMode.Transparent;
            chart.Title.IsAutomaticSize = true;
            chart.Title.Height = 100;
            chart.Title.Width = 200;
            chart.Title.Shadow = false;

            // Сохраните книгу
            workbook.Save("TitleExample.xlsx");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



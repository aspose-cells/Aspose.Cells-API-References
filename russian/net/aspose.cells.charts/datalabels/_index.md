---
title: "Класс DataLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Charts.DataLabels. Инкапсулирует коллекцию всех объектов DataLabel для указанной серии"
type: docs
url: /ru/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Инкапсулирует коллекцию всех объектов DataLabel для указанной серии.

```csharp
public class DataLabels : ChartTextFrame
```

## Свойства

| Имя | Описание |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Получает [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | True, если текст в объекте изменяет размер шрифта при изменении размера объекта. Значение по умолчанию — True. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Получает и задает режим отображения фона. Это свойство действительно только в Excel 2003 и более ранних версиях. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Получает и задает режим отображения фона |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Получает [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Представляет высоту положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Представляет высоту положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Представляет ширину положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Представляет ширину положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Представляет координату x положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Представляет координату x положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Представляет координату y положения по умолчанию в единицах 1/4000 области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Представляет координату y положения по умолчанию в единицах доли области диаграммы. (Наследовано от [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Получает и задает направление текста. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Получает шрифт DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Получает или задает высоту кадра в единицах 1/4000 области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Получает или задает высоту кадра в пикселях.(Наследовано от [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Получает или задает высоту кадра в единицах отношения к области диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Указывает, автоматически ли вращается текст диаграммы.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Указывает, автоматически ли задаются размеры кадра диаграммы.(Наследовано от [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Указывает, что текст сгенерирован автоматически. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Указывает, установлена ли позиция по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight).(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Указывает, удалена ли эта метка данных.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Указывает, включает ли размер области построения отметки делений и подписи осей. Значение False указывает, что размер определяет только область построения, без отметок делений и подписей осей.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Указывает, будет ли Datalabels никогда не перекрываться при преобразовании круговой диаграммы в изображение. Примечание: это свойство имеет смысл только при преобразовании круговой диаграммы в изображение. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Получает или задает, должна ли форма автоматически подгоняться, чтобы полностью содержать описанный в ней текст. Автоподгонка — это масштабирование текста внутри формы для размещения всего текста внутри.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Получает или задает значение, указывающее, будет ли текст переноситься. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Получает и задает ссылку на лист рабочей книги.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Получает и задает встроенный числовой формат. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Представляет строку формата для объекта DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | True, если числовой формат связан с ячейками (чтобы формат числа менялся в метках, когда он меняется в ячейках). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Представляет позицию метки данных. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Представляет порядок чтения текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Представляет угол поворота текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Получает или задает тип разделителя, используемого для меток данных на диаграмме. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Получает или задает значение разделителя, используемого для меток данных на диаграмме. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | True, если у кадра есть тень.(Наследовано от [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Получает объект [`ShapeProperties`](../chartframe/shapeproperties/).(Наследовано от [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Получает или задает тип формы метки данных. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Представляет поведение отображения процентного значения метки данных указанной диаграммы. True отображает процентное значение. False скрывает процентное значение. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Представляет поведение отображения названия категории метки данных указанной диаграммы. True для отображения названия категории для меток данных на диаграмме. False для скрытия. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Указывает, следует ли отображать диапазон ячеек в качестве меток данных. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Представляет поведение отображения ключа легенды метки данных указанной диаграммы. True, если ключ легенды метки данных видим. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Представляет поведение отображения процентного значения метки данных указанной диаграммы. True отображает процентное значение. False скрывает. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Указывает, отображается ли имя серии в метках данных на диаграмме. True — показывать имя серии. False — скрывать. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Представляет поведение отображения значений метки данных указанной диаграммы. True отображает значения. False скрывает. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Получает или задает текст метки данных. |
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
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Применить шрифт меток данных ко всем дочерним узлам. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Возвращает объект Characters, представляющий диапазон символов внутри текста.(Наследовано от [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Устанавливает позицию рамки в автоматический режим(Наследовано от [`ChartFrame`](../chartframe/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DataLabelsDemo
    {
        public static void DataLabelsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
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

            // Добавить серию к диаграмме
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить доступ к DataLabels первой серии
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Установить свойства DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Сохраните книгу
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
    }
}
```

### См. также

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



---
title: DataLabels
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует коллекцию всех объектов DataLabel для указанной серии.
type: docs
weight: 580
url: /ru/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Инкапсулирует коллекцию всех объектов DataLabel для указанной серии.

```csharp
public class DataLabels : ChartTextFrame
```

## Характеристики

| Имя | Описание |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area) { get; } | Получает[`область`](./area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Истинно, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию верно. |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode) { get; set; } | Получает и устанавливает режим отображения background |
| override [Border](../../aspose.cells.charts/datalabels/border) { get; } | Получает[`граница`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Представляет высоту позиции по умолчанию |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Представляет ширину позиции по умолчанию |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Представляет x позиции по умолчанию |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Представляет y позиции по умолчанию |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype) { get; set; } | Получает и задает направление текста. |
| override [Font](../../aspose.cells.charts/datalabels/font) { get; } | Получает шрифт DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Получает или задает высоту кадра в единицах 1/4000 области диаграммы. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Указывает, имеет ли рамка диаграммы автоматический размер. |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext) { get; set; } | Указывает, что текст генерируется автоматически. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Указывает, установлены ли позиции по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Указывает, удалены ли эти метки данных. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Указывает, включает ли размер области графика деления и метки осей. False указывает, что размер должен определять размер области графика, деления и метки осей. |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap) { get; set; } | Указывает, никогда не перекрываются отображаемые метки данных. (Для круговой диаграммы) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Получает или задает значение, указывающее, должна ли фигура автоматически подбираться, чтобы полностью содержать описанный в ней текст. Автоматическая подгонка is , когда текст внутри фигуры масштабируется, чтобы содержать весь текст внутри. |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped) { get; set; } | Получает или задает значение, указывающее, переносится ли текст. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Получает и устанавливает ссылку на рабочий лист. |
| [Number](../../aspose.cells.charts/datalabels/number) { get; set; } | Получает и задает встроенный числовой формат. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat) { get; set; } | Представляет строку формата для объекта DataLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked) { get; set; } | Истинно, если числовой формат привязан к ячейкам (чтобы числовой формат менялся в метках при изменении в ячейках). |
| [Position](../../aspose.cells.charts/datalabels/position) { get; set; } | Представляет положение метки данных. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Представляет порядок чтения текста. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Представляет угол поворота текста. |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype) { get; set; } | Получает или задает тип разделителя, используемый для меток данных на диаграмме. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue) { get; set; } | Получает или задает значение разделителя, используемое для меток данных на диаграмме. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Истинно, если у кадра есть тень. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Получает[`ShapeProperties`](../chartframe/shapeproperties) объект. |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype) { get; set; } | Получает или задает тип формы метки данных. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize) { get; set; } | Представляет поведение отображения процентного значения метки данных указанной диаграммы. True отображает процентное значение. Ложь скрывать. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname) { get; set; } | Представляет поведение отображения имени категории меток данных указанной диаграммы. Значение true для отображения имени категории для меток данных на диаграмме. Ложь, чтобы скрыть. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange) { get; set; } | Указывает, отображается ли диапазон ячеек в качестве меток данных. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey) { get; set; } | Представляет поведение отображения ключа легенды метки данных указанной диаграммы. Истинно, если ключ легенды метки данных виден. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage) { get; set; } | Представляет поведение отображения процентного значения метки данных указанной диаграммы. True отображает процентное значение. Ложь скрывать. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname) { get; set; } | Возвращает или задает логическое значение, чтобы указать поведение отображения имени ряда для меток данных на диаграмме. Истинно, чтобы показать имя ряда. Ложь, чтобы скрыть. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue) { get; set; } | Представляет поведение отображения значений меток данных указанной диаграммы. True отображает значения. Ложь скрывать. |
| override [Text](../../aspose.cells.charts/datalabels/text) { get; set; } | Получает или задает текст метки данных. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Получает и задает выравнивание текста по горизонтали. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Получает или задает выравнивание текста по вертикали. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Получает или задает ширину рамки в единицах 1/4000 области диаграммы. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Получает или задает координату x левого верхнего угла в единицах 1/4000 области диаграммы. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Получает или задает координату Y верхнего левого угла в единицах 1/4000 области диаграммы. |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Возвращает объект символов, представляющий диапазон символов в тексте. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Установить положение кадра на auto |

### Примеры

```csharp

[C#]

//Устанавливаем метки данных на диаграмме
DataLabels datalabels;
for (int i = 0; i  <chart.NSeries.Count; i++)
{
    datalabels = chart.NSeries[i].DataLabels;
    //Устанавливаем положение DataLabels
    datalabels.Position = LabelPositionType.InsideBase;
    //Показать название категории в DataLabels
    datalabels.ShowCategoryName = true;
    //Показать значение в DataLabels
    datalabels.ShowValue = true;
    //Не показывать процент в DataLabels
    datalabels.ShowPercentage = false;
    //Не показывать ключ легенды.
    datalabels.ShowLegendKey = false;
}

[Visual Basic]

'Установите метки данных на диаграмме
Dim datalabels As DataLabels
Dim i As Integer
For i = 0 To chart.NSeries.Count - 1 Step 1
    datalabels = chart.NSeries(i).DataLabels
    'Установите положение DataLabels
    datalabels.Position = LabelPositionType.InsideBase
    'Показать название категории в DataLabels
    datalabels.ShowCategoryName= True
    'Показать значение в DataLabels
    datalabels.ShowValue = True
    'Не показывать процент в DataLabels
    datalabels.ShowPercentage = False
    'Не показывать ключ легенды.
    datalabels.ShowLegendKey = False
Next
```

### Смотрите также

* class [ChartTextFrame](../charttextframe)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

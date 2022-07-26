---
title: Legend
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий легенду диаграммы.
type: docs
weight: 690
url: /ru/net/aspose.cells.charts/legend/
---
## Legend class

Инкапсулирует объект, представляющий легенду диаграммы.

```csharp
public class Legend : ChartTextFrame
```

## Характеристики

| Имя | Описание |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Получает[`область`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Истинно, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию верно. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Получает и устанавливает режим отображения background |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Получает[`граница`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Представляет высоту позиции по умолчанию |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Представляет ширину позиции по умолчанию |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Представляет x позиции по умолчанию |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Представляет y позиции по умолчанию |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Получает и задает направление текста. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Получает[`Font`](../chartframe/font) объект указанного объекта ChartFrame. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Получает или задает высоту кадра в единицах 1/4000 области диаграммы. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Указывает, имеет ли рамка диаграммы автоматический размер. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Указывает, что текст генерируется автоматически. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Указывает, установлены ли позиции по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Указывает, удалены ли эти метки данных. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Указывает, включает ли размер области графика деления и метки осей. False указывает, что размер должен определять размер области графика, деления и метки осей. |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Получает или задает, разрешено ли другим элементам диаграммы перекрывать этот элемент диаграммы. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Получает или задает значение, указывающее, должна ли фигура автоматически подбираться, чтобы полностью содержать описанный в ней текст. Автоматическая подгонка is , когда текст внутри фигуры масштабируется, чтобы содержать весь текст внутри. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Получает или задает значение, указывающее, переносится ли текст. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Получает коллекцию всех объектов LegendEntry в указанной легенде диаграммы. Установка записей легенды для поверхностной диаграммы не поддерживается. Таким образом, будет возвращено значение null, если тип диаграммы является типом поверхностной диаграммы. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Получает метки записей легенды после вызова метода Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Получает и устанавливает ссылку на рабочий лист. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Получает или задает тип позиции легенды. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Представляет порядок чтения текста. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Представляет угол поворота текста. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Истинно, если у кадра есть тень. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Получает[`ShapeProperties`](../chartframe/shapeproperties) объект. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Получает или задает текст заголовка фрейма. |
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
   
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
//Устанавливаем ширину и высоту легенды
Legend legend = chart.Legend;

//Легенда по умолчанию находится справа от графика.
//Если легенда находится слева или справа от графика, установка свойства Legend.X не вступит в силу.
//Если легенда находится в верхней или нижней части графика, установка свойства Legend.Y не вступит в силу.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
//Установить положение легенды
legend.Position = LegendPositionType.Left;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'Легенда по умолчанию находится справа от диаграммы.
'Если легенда находится слева или справа от диаграммы, установка свойства Legend.X не вступит в силу.
'Если легенда находится вверху или внизу диаграммы, установка свойства Legend.Y не вступит в силу.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### Смотрите также

* class [ChartTextFrame](../charttextframe)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

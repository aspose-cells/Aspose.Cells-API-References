---
title: Title
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий заголовок диаграммы или оси.
type: docs
weight: 970
url: /ru/net/aspose.cells.charts/title/
---
## Title class

Инкапсулирует объект, представляющий заголовок диаграммы или оси.

```csharp
public class Title : ChartTextFrame
```

## Характеристики

| Имя | Описание |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Получает[`area`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Истинно, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию верно. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Получает и устанавливает режим отображения фона |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Получает[`border`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Представляет высоту позиции по умолчанию |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Представляет ширину позиции по умолчанию |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Представляет x позиции по умолчанию |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Представляет y позиции по умолчанию |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Получает и задает направление текста. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Получает объект[`Font`](../chartframe/font)указанного объекта ChartFrame. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Получает или задает высоту рамки в единицах 1/4000 области диаграммы. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Указывает, имеет ли рамка диаграммы автоматический размер. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Указывает, что текст генерируется автоматически. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Указывает, установлены ли позиции по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Указывает, удалены ли эти метки данных. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Указывает, включает ли размер области графика деления и метки осей. False указывает, что размер должен определять размер области графика, делений и меток осей. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Получает или задает значение, указывающее, должна ли фигура автоматически подбираться, чтобы полностью содержать описанный в ней текст. Автоматическая подгонка когда текст внутри фигуры масштабируется, чтобы содержать весь текст внутри. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Получает или задает значение, указывающее, переносится ли текст. |
| [IsVisible](../../aspose.cells.charts/title/isvisible) { get; set; } | Указывает, виден ли заголовок. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Получает и устанавливает ссылку на рабочий лист. |
| [OverLay](../../aspose.cells.charts/title/overlay) { get; set; } | Представляет наложение заголовка по центру на диаграмме без изменения размера диаграммы. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Представляет порядок чтения текста. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Представляет угол поворота текста. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Истинно, если у кадра есть тень. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Получает объект[`ShapeProperties`](../chartframe/shapeproperties). |
| override [Text](../../aspose.cells.charts/title/text) { get; set; } | Получает или задает текст метки единицы отображения. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Получает и задает выравнивание текста по горизонтали. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Получает или задает выравнивание текста по вертикали. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Получает или задает ширину рамки в единицах 1/4000 области диаграммы. |
| override [X](../../aspose.cells.charts/title/x) { get; set; } | Получает или задает координату x левого верхнего угла в единицах 1/4000 области диаграммы. |
| override [Y](../../aspose.cells.charts/title/y) { get; set; } | Получает или задает координату Y верхнего левого угла в единицах 1/4000 области диаграммы. |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters#characters_1)() | Получает расширенное форматирование текста этого заголовка. |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Возвращает объект Characters, представляющий диапазон символов в тексте. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Установить положение кадра автоматически |

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

  //Установка заголовка диаграммы
chart.Title.Text = "Title";
  //Установка цвета шрифта заголовка диаграммы на blue
chart.Title.Font.Color = Color.Blue;
  //Установка заголовка оси категорий диаграммы
chart.CategoryAxis.Title.Text = "Category";
  //Установка заголовка оси значений диаграммы
chart.ValueAxis.Title.Text = "Value";

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
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)      ///
Dim chart as Chart = sheet.Charts(chartIndex)

'Setting the title of a chart
chart.Title.Text = "Title"
'Setting the font color of the chart title to blue
chart.Title.Font.Color = Color.Blue
'Setting the title of category axis of the chart
chart.CategoryAxis.Title.Text = "Category"
'Setting the title of value axis of the chart
chart.ValueAxis.Title.Text = "Value"

```

### Смотрите также

* class [ChartTextFrame](../charttextframe)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

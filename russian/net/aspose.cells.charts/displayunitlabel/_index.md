---
title: DisplayUnitLabel
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет метку устройства отображения.
type: docs
weight: 600
url: /ru/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Представляет метку устройства отображения.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Характеристики

| Имя | Описание |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Получает[`area`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | Истинно, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию верно. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Получает и устанавливает режим отображения фона |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Получает[`border`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Представляет высоту позиции по умолчанию |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Представляет ширину позиции по умолчанию |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Представляет x позиции по умолчанию |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Представляет y позиции по умолчанию |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Получает и задает направление текста. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | Получает объект[`Font`](./font)указанного объекта ChartFrame. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Получает или задает высоту рамки в единицах 1/4000 области диаграммы. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Указывает, имеет ли рамка диаграммы автоматический размер. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Указывает, что текст генерируется автоматически. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Указывает, установлены ли позиции по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Указывает, удалены ли эти метки данных. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Указывает, включает ли размер области графика деления и метки осей. False указывает, что размер должен определять размер области графика, делений и меток осей. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Получает или задает значение, указывающее, должна ли фигура автоматически подбираться, чтобы полностью содержать описанный в ней текст. Автоматическая подгонка когда текст внутри фигуры масштабируется, чтобы содержать весь текст внутри. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Получает или задает значение, указывающее, переносится ли текст. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Получает и устанавливает ссылку на рабочий лист. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Представляет порядок чтения текста. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Представляет угол поворота текста. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Истинно, если у кадра есть тень. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Получает объект[`ShapeProperties`](../chartframe/shapeproperties). |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Получает или задает текст метки единицы отображения. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Получает и задает выравнивание текста по горизонтали. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Получает или задает выравнивание текста по вертикали. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Получает или задает ширину рамки в единицах 1/4000 области диаграммы. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Получает или задает координату x левого верхнего угла в единицах 1/4000 области диаграммы. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Получает или задает координату Y верхнего левого угла в единицах 1/4000 области диаграммы. |

## Методы

| Имя | Описание |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Возвращает объект Characters, представляющий диапазон символов в тексте. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Установить положение кадра автоматически |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  //Добавление нового рабочего листа в Excel object
int sheetIndex = workbook.Worksheets.Add();
  //Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
  //Добавление значения выборки в "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Добавление значения образца в "A2" cell
worksheet.Cells["A2"].PutValue(100);
  //Добавление значения образца в "A3" cell
worksheet.Cells["A3"].PutValue(150);
  //Добавление образца значения в "A4" cell
worksheet.Cells["A4"].PutValue(200);
  //Добавление образца значения в "B1" cell
worksheet.Cells["B1"].PutValue(60);
  //Добавление значения образца в "B2" cell
worksheet.Cells["B2"].PutValue(32);
  //Добавление значения образца в "B3" cell
worksheet.Cells["B3"].PutValue(50);
  //Добавление значения образца в "B4" cell
worksheet.Cells["B4"].PutValue(40);
  //Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells["C1"].PutValue("Q1");
  //Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells["C2"].PutValue("Q2");
  //Добавление значения образца в ячейку "C3" как категория data
worksheet.Cells["C3"].PutValue("Y1");
  //Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells["C4"].PutValue("Y2");
  //Добавление диаграммы на лист
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
  //Доступ к экземпляру только что добавленного chart
Chart chart = worksheet.Charts[chartIndex];
  //Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
chart.NSeries.Add("A1:B4", true);
  //Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4";
  //Установка единицы отображения значения (Y) оси.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
  //Установка пользовательской единицы отображения label
displayUnitLabel.Text = "100";
  //Сохранение файла Excel
workbook.Save("book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adding a chart to the worksheet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Setting the data source for the category data of NSeries
Chart.NSeries.CategoryData = "C1:C4"
'Setting the display unit of value(Y) axis.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Setting the custom display unit label
displayUnitLabel.Text = "100"
'Saving the Excel file
workbook.Save("book1.xls")
```

### Смотрите также

* class [ChartTextFrame](../charttextframe)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
